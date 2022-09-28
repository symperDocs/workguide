# Concept



## **CÁCH SỬ DỤNG CÔNG THỨC TRONG DOCUMENT**

### **Công thức truy vấn dữ liệu đến CSDL**

Công thức thức truy vấn đến CSDL là dạng công thức sử dụng để truy cập và lấy dữ liệu đã được lưu trữ ở phía CSDL (symper đang sử dụng database **postgres** nên cú pháp và các hàm sẽ sử dụng của **postgreSQL**)

{% hint style="info" %}
[Truy cập document của postgresQL ở đây](https://www.postgresql.org/docs/)
{% endhint %}

**Ví dụ:** Đối với các bản ghi đã được submit trên document thì các bản ghi đấy đã được người dùng thực hiện hành động lưu lại, và bản ghi đó được lưu trữ trong CSDL trên server của hệ thống symper.

![](https://lh5.googleusercontent.com/MtKtjztux4-FrUL-Jw7y-cLjZH\_FrwKlh0T3Lv0FywMW9Hp7Ro8ZX99VjIsu0pOzHq9vPUgTbT5dhcocHXUmN77nnvYgQxNNrP3yjcHmu\_g2cwimXVwvItO7VjH69\_\_bNNay8oib)

Hình trên là ví dụ của danh sách các bản ghi đã được lưu trữ lại thông qua hành động submit của người dùng.

Trong quá trình xây dựng các module nghiệp vụ sẽ phát sinh nhu cầu truy cập vào CSDL đã có để lấy thông tin phục vụ quá trình tính toán, hiển thị. Công thức sử dụng để truy vấn đến CSDL của hệ thống symper sẽ giải quyết vấn đề này.

Để phân loại với các cú pháp phục vụ các mục đích khác, công thức truy vấn về CSDL sẽ có một wrapper xác định trước là `ref(syntax)`. Toàn bộ công thức thức sẽ được viết trong `ref()`, khi đó hệ thống sẽ tự động phát hiện công thức có chứa wrapper ref và đẩy về phía server để thực thi câu lệnh**.**

![](https://lh5.googleusercontent.com/EFnyzi4kUynmjdVp4AMJ9qw-SY0C2DEIhHg8ek-SJc12ShKzECaMnzexn3xCUyJJJXZXz7MpfZ6ASuBe3G86-6NIbKQWeQza\_1gMjCnYyqt444VZhjLvIv88Wc70ZCfywK3LkS\_x)

Ví dụ về một công thức truy vấn các bản ghi đã được lưu trữ để phục vụ người dùng nhập liệu.

```sql
ref(
        select name_assignee as "Ng làm", 
            wbs_id as wbs_depe, 
            tmg_name as "Mô tả WBS", 
            ngay_start as "NCT" 
        from symper_wbs 
        where (wbs_id ilike '%{wbs_depe}%' or tmg_description ilike '%{wbs_depe}%') 
                and document_object_user_created_id = {CURRENT_USER_ID} 
        order by ngay_start desc 
        limit 40 offset 0 
)
```

Sử dụng tham số để làm điều kiện truy vấn

Trong thực tế, các document sẽ cần sử dụng các thông tin mà người dùng nhập vào để làm điều kiện truy vấn đến dữ liệu mong muốn trên CSDL**.**&#x20;

**Ví dụ:** Khi người dùng nhập mã module là DO, thì ở trường thông tin submodule chỉ hiển thị ra các submodule của Module lớn mà người dùng đã chọn là DO.

![](https://lh3.googleusercontent.com/hEm9Mpiq4Xz9PSrKv1kJ9tutZzY1To3sHXio8-B0pYfzc3\_j4NdG-UooLNhcla5OZZ\_xOA7zqzHvUA51Y-BBA6INmgvFBJHquCmkgB6XOFoI8dO0LlQ7XsfCEZ88D6iNfusnhvLN)

Về logic việc sử dụng công thức để giải quyết bài toán này là truy vấn về CSDL submodule và điều kiện lấy dữ liệu là module bằng ‘DO’. Để giải quyết bài toán này BA cần viết công thức truy vấn về server và điều kiện lấy dữ liệu là tham số của người dùng nhập vào.

**Cú pháp:**  Cú pháp được sử dụng để lấy tham số người dùng nhập vào là **** `{ten_truong_thong_tin}`

Vậy cú pháp để giải quyết bài toán trên: ****&#x20;

```sql
select submodule from dm_module where module = ‘{ten_truong_thong_tin}’
```

![](https://lh3.googleusercontent.com/PG6es-rgkUNy9byPVIgpm3s8NDL69zOKqCpQ5CpNF6Oh7rf6U41k\_-f2\_8W\_RuYFQD5sjyGO-9uaaAPc-GPxPSicHUvV3\_m3VLwgC\_2Q9cLGF7ssMKkrb7XN5sV-wBnmx31iDlrL)

Sử dụng thêm cặp `‘’` để xác định kiểu dữ liệu là `text` (text hoặc date), đối với kiểu là `number` thì không cần sử dụng `‘’`.

Khi hệ thống biên dịch cú pháp trên bước đầu tiên sẽ tìm kiếm các trường thông tin nằm trong dấu `{}` để thay thế bằng các giá trị của biển số thực tế, sau đấy xác định có wrapper `ref` hay không để chuyển về server thực thi. Cú pháp công thức sau khi biến số trong `{}` được thay thế bằng giá trị trong trường hợp nêu trên:&#x20;

```sql
select submodule from dm_module where module = ‘DO’
```

### **Lấy dữ liệu cho control trong table**

Đối với control trong table, việc lấy dữ liệu trên server để tạo ra dữ liệu cho cột dữ liệu và row dữ liệu trong table với điều kiện là một cột dữ liệu khác ngay trong table mà người dùng nhập liệu hoàn toàn có thể thực hiện bằng cấu trúc truy vấn về server.\
****

![](https://lh5.googleusercontent.com/uzT8WggBYH-p756EaUbdJNp1RCGSu5i3D4rIUJAXhWyDKnAEEwu-D6v9ggbIpquoMVUpl-gww1eVUhBKY95\_8nC3SPptiNuFilMVIGRtovpv6hiq-skrZEQWEWZxUIy0rQ0WnPEF)

```sql
ref(
    SELECT ten_hang as tb1_ten_hang 
    from dm_hhdv 
    where ma_hang = '{tb1_ma_hang}'
)
```

tham số là cột `tb1_ma_hang`, cách viết công thức này sẽ giúp khi người dùng nhập mã hàng hoá vào cột mã hàng thì 2 cột tên hàng hoá và đơn vị tính sẽ tự động lấy dữ liệu từ bảng danh mục hàng hoá ở server. công thức sẽ được apply cho toàn bộ các row trong table mà người dùng thêm vào, và sẽ thực thi cùng một câu lệnh, các biến số sẽ được thay thế theo row tương ứng nếu như BA có sử dụng một control trong table làm biến số.

### **Công thức truy vấn trên client**

Công thức truy vấn trên client là các công thức sử dụng để thực thi tính toán, logic, lấy dữ liệu mà user đang nhập vào document ngay tại thời điểm user nhập liệu. Công thức đối với truy vấn trên client không cần sử dụng wrapper**.**

Có 2 kiểu truy vấn trên client cơ bản: kiểu thứ nhất là việc tính toán giữa các control ngoài table khi người dùng nhập liệu, kiểu thứ 2 tính toán dữ liệu mà người dùng nhập vào control table trong document.

**Công thức truy vấn trên client cho control nằm ngoài table**

**Ví dụ 1:** Lấy ngày hiện tại, ví dụ về việc tạo ra dữ liệu cho input bằng công thức client

![](https://lh5.googleusercontent.com/B1AsWvzYqiQm7TgV7rDCv6wgI-Z-68mc6wPDrBgpA7d94MUVlLGdJbn6N\_vWcdGLmcW3\_61xSbFQIklPxXzbAcp9DVJGpVxzHI\_fgZb8Sm95BpTfTe4ZQJ-CPcIjS5tZc\_E3AU9s)

```sql
SELECT date('now')
```

Trong form nhập liệu trên khi người dùng đăng nhập vào trường thông tin ngày phát sinh sẽ tự động lấy ngày hiện tại mà không cần phải nhập liệu.

**Ví dụ 2:** Trường thông tin diễn giải trong document sẽ được tạo ra bằng cách ghép các thông tin từ những trường thông tin khác mà người dùng nhập vào

![](https://lh5.googleusercontent.com/PecjDed6aP7YnvZarBmC1vloR6zycRbmBhiba4BFEG053sjIAGzStzDd8MgV8dmK6PF6PsUNBo3ergrqzCvESlh-wmK\_YnFR0l9Z15CRVTe9XWluUPGMKJAH1IFHzsz42s33LxFf)

Về cơ bản, hệ thống sẽ sử dụng cơ chế biên dịch (thay thế giá trị) vào các biến được xác định thông qua dấu **`{}`**

**Công thức truy vấn trên client vào table có trong doc**

Dữ liệu được người dùng nhập vào một table có trong doc sẽ có cấu trúc như một table trong CSDL (có các row và columns). Vì vậy để giải quyết bài toán sử dụng dữ liệu đã được nhập vào trong table để tính toán về cơ bản có cùng chung tư tưởng với việc truy vấn đến CSDL ở mục 1, điểm khác biệt duy nhất CSDL được lưu trữ trên server, table trên client được lưu trữ tại máy của người dùng. ****&#x20;

Để giải quyết nhu cầu trên, đối với các document có table, hệ thống symper sẽ tự động tạo ra các bảng lưu trữ dữ liệu vật lý với đúng cấu trúc như của table trong document (số lượng row, số lượng columns) với tên của bảng dữ liệu chính là tên của control table. Hệ quản trị CSDL sử dụng **SQLite** vì vậy cấu trúc và các hàm sử dụng là **SQLite**. Cấu trúc truy vấn sẽ sử dụng đúng cấu trúc của **SQLite**.

{% hint style="info" %}
[Truy cập document của SQLite ở đây](https://www.sqlite.org/index.html)
{% endhint %}

![](https://lh4.googleusercontent.com/wkhCG8mGH2ksL\_H\_1r49B4ff4VA39SQpzIPTu9nFQoIWlOTJbjnq\_t9USHJUT9we2Wz0d9CF3bKplbMptuC6XkTaN4fEXs-sDXXwALbqo1qqnWxFii1Qe1u5cJmjGGuVAf6YH4sI)

Với ví dụ trên, document phiếu nhu cầu có 1 table về hàng hoá mua, hệ thống sẽ tự động tạo ra 1 bảng lưu trữ dữ liệu vật lý ngay trên client với số lượng row và columns bằng đúng với số lượng cột của table và số lượng dòng dữ liệu mà người dùng nhập liệu vào.

![](https://lh6.googleusercontent.com/Ve4-dBR8c1ycyTrCY9ueaFUUN-Mzu7J1Z6GYF3MhB1JzSuRoWdMj-q4Sen7OtnghAqSUEydLCMytfv50WHnViAaA4thd9pZCcYvi1eag4emx-emvrN2JNvUz7Tw5dodoEwHrAcsn)

```sql
select sum(tb1_sl_yc) from tb1
```

**Ví dụ:** trong document phiếu nhu cầu có một trường thông tin ngoài table để tính tổng số lượng yêu cầu, BA có thể viết cấu trúc truy vấn vào bảng dữ liệu lưu trữ tại client thông qua cấu trúc của **SQLite.**

### **Công thức tính toán giữa các cột trong table**

![](https://lh4.googleusercontent.com/o8Ftvxo\_bzeRSAh\_vtPxa1s-z4xna0z8pPbsgu4woMHffyAY8uzTgcZoNKwQeI98y7MWhSo5BchDRWl2sMygHxad9iD2LhIn8pV92Cnu1HL7IX\_GbitBlh7Ocw9UZoQJMYqRML77)

**Ví dụ:** trong document phía trên ta có trường số lượng và trường đơn giá, trường thành tiền, trường thành tiền sẽ bằng trường đơn giá nhân số lượng theo row.

Để xử lý bài toán này chỉ cần viết công thức thực thi trên client bằng cách lấy cột số lượng nhân với cột đơn giá (Luôn dùng từ khoá select để bắt đầu một công thức lấy dữ liệu)

![](https://lh3.googleusercontent.com/zgVdI8CUGMzRJC8cYVoDxD6t9ZOXpX1mm8hpSx7\_8ZbhYTvcK7qXwuH7wgYTzXV6uYDfHd50pitBLAqwLNH16Gn3wCk3t85eNNwxAzaD6iNeyaQpA5mj7qbC68o02q4EGHq7VF2K)

```sql
select {tb1_sl_bl} * {tb1_gia_nt}
```
