---
description: Duyenntm
---

# Kiểm thử hộp đen

## 1. Khái niệm

_**Kiểm thử hộp đen**_ là một phương pháp kiểm thử phần mềm được thực hiện mà không biết được cấu tạo bên trong của phần mềm, là cách mà các tester kiểm tra xem hệ thống như một chiếc hộp đen, không có cách nào nhìn thấy bên trong của cái hộp.

* Nó còn được gọi là kiểm thử hướng dữ liệu hay là kiểm thử hướng in/out.
* Người kiểm thử nên xây dựng các nhóm giá trị đầu vào mà sẽ thực thi đầy đủ tất cả các yêu cầu chức năng của chương trình.
* Cách tiếp cận của các tester đối với hệ thống là không dùng bất kỳ một kiến thức về cấu trúc lập trình bên trong hệ thống, xem hệ thống là một cấu trúc hoàn chỉnh, không thể can thiệp vào bên trong.

![](<../.gitbook/assets/image (3).png>)

Black Box Testing chủ yếu là được thực hiện trong Function test và System test.

## **2. Đặc điểm và mục đích của kiểm thử hộp đen**

### 2.1. Đặc điểm của kiểm thử hộp đen:&#x20;

* Bổ xung cho phương pháp kiểm thử hộp trắng để phát hiện ra tất cả các lỗi khác nhau mà kiểm thử hộp trắng không phát hiện ra được.
* Không cần quan tâm đến thiết kế, mã nguồn mà chỉ quan tâm đến chức năng đã đề ra của chương trình.
* Chỉ dựa vào bản mô tả chức năng của chương trình.
* Hướng vào các đặc tả bên ngoài.
* Chủ yếu là kiểm tra giao diện.
* Áp dụng vào giai đoạn sau của vòng kiểm thử.

### 2.2. Mục đích của kiểm thử hộp đen là tìm các lỗi sai liên quan đến:

* Chức năng không chính xác hoặc thiếu.
* Lỗi giao diện.
* Lỗi trong cấu trúc dữ liệu hoặc truy cập cơ sở dữ liệu bên ngoài.
* Hành vi hoặc hiệu suất lỗi.
* Khởi tạo và chấm dứt các lỗi.

## 3. Ưu điểm và nhược điểm của kiểm thử hộp đen

**Ưu điểm:**

* Các tester được thực hiện từ quan điểm của người dùng và sẽ giúp đỡ trong việc sáng tỏ sự chênh lệch về thông số kỹ thuật.
* Các tester theo phương pháp black box không có “mối ràng buộc” nào với code, và nhận thức của một tester rất đơn giản: một source code có nhiều lỗi. Sử dụng nguyên tắc, "Hỏi và bạn sẽ nhận" các tester black box tìm được nhiều bug ở nơi mà các DEV không tìm thấy.
* Tester có thể không phải IT chuyên nghiệp, không cần phải biết ngôn ngữ lập trình hoặc làm thế nào các phần mềm đã được thực hiện.
* Các tester có thể được thực hiện bởi một cơ quan độc lập từ các developer, cho phép một cái nhìn khách quan và tránh sự phát triển thiên vị.
* Hệ thống thật sự với toàn bộ yêu cầu của nó được kiểm thử chính xác.
* Thiết kế kịch bản kiểm thử khá nhanh, ngay khi mà các yêu cầu chức năng được xác định.

**Nhược điểm:**

* Dữ liệu đầu vào yêu cầu một khối lượng mẫu (sample) khá lớn
* Nhiều dự án không có thông số rõ ràng thì việc thiết kế test case rất khó và do đó khó viết kịch bản kiểm thử do cần xác định tất cả các yếu tố đầu vào, và thiếu cả thời gian cho việc tập hợp này.
* Khả năng để bản thân kỹ sư lạc lối trong khi kiểm thử là khá cao.
* Chỉ có một số nhỏ các đầu vào có thể được kiểm tra và nhiều đường dẫn chương trình sẽ được để lại chưa được kiểm tra.
* Kiểm thử black box được xem như "là bước đi trong mê cung tối đen mà không mang đèn pin” bởi vì tester không biết phần mềm đang test đã được xây dựng như thế nào. Có nhiều trường hợp khi một tester viết rất nhiều trường hợp test để kiểm tra một số thứ có thể chỉ được test bằng một trường hợp test và/hoặc một vài phần cuối cùng không được test hết.

## 4. Sự k**hác nhau giữa kiểm thử hộp đen và hộp trắng**

![Sự khác biệt giữa kiểm thử hộp đen và khiểm thử hộp trắng](<../.gitbook/assets/image (1).png>)

|                                      | Kiểm thử hộp đen                                                                                                                                       | Kiểm thử hộp trắng                                                                                                                          |
| ------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------- |
| **Định nghĩa**                       | Kiểm tra hộp đen là phương pháp thử nghiệm phần mềm được ѕử dụng để đánh giá những phần mềm mà không quan tâm tới cấu trúc bên trong của chương trình. | Kiểm tra hộp trắng là phương pháp kiểm thử phần mềm, ѕử dụng để kiểm tra phần mềm mà уêu cầu phải biết cấu trúc bên trong của chương trình. |
| **Trách nhiệm**                      | Thử nghiệm được thực hiện bên ngoài, không liên quan đến nhà phát triển phần mềm.                                                                      | Thông thường, các thử nghiệm được thực hiện bởi nhà phát triển phần mềm.                                                                    |
| **Cấp độ teѕt ѕử dụng**              | Thử nghiệm áp dụng ở cấp độ cao như: đánh giá hệ thống (Sуѕtem teѕt), kiểm tra chấp nhận (Acceptance teѕt)                                             | Thử nghiệm được áp dụng ở mức độ thấp hơn như thử nghiệm đơn ᴠị (Unit Teѕt), thử nghiệm hội nhập (Integration teѕt)                         |
| **Biết lập trình**                   | Không уêu cầu hiểu biết ᴠề Lập trình                                                                                                                   | Yêu cầu hiểu biết nhất định ᴠề lập trình.                                                                                                   |
| **Biết ᴠiệc thực hiện chương trình** | Không уêu cầu hiểu ᴠề cấu trúc bên trong chức năng, ᴠà không cẩn hiểu làm thế nào để có được chức năng đó                                              | Yêu cầu hiểu cấu trúc bên trong chức năng được thực hiện như nào.                                                                           |
| **Cơ ѕở tạo Teѕt Caѕeѕ**             | Kiểm tra hộp đen được bắt đầu dựa trên tài liệu уêu cầu kỹ thuật                                                                                       | Kiểm tra hộp trắng được bắt đầu dựa trên các tài liệu thiết kế chi tiết                                                                     |

## 5. Các kỹ thuật test thường dùng trong kiểm thử hộp đen

### 5.1. Phân vùng tương đương (Equivalence Class Partitioning)

Phân vùng lớp tương đương cho phép bạn phân chia tập hợp các điều kiện kiểm tra thành một phân vùng nên được coi là giống nhau.

Phương pháp kiểm thử phần mềm này chia miền đầu vào của chương trình thành các lớp dữ liệu mà từ đó các trường hợp kiểm thử nên được thiết kế.

_**Với các giá trị đầu vào chia thành các vùng tương đương:**_

* Vùng tương đương hợp lệ: tập hợp các giá trị kiểm thử thỏa mãn điều kiện của hệ thống
* Vùng tương đương không hợp lệ: Tập hợp các giá trị kiểm thử mô tả trạng thái khác của hệ thống: sai, thiếu, không đúng,...

_**Mục đích:**_ Giảm đáng kể số lượng test case cần phải thiết kế vì với mỗi lớp tương đương ta chỉ cần test trên các phần tử đại diện.

_**Thiết kế Test-case bằng phân lớp tương đương tiến hành theo 2 bước:**_

* Xác định các lớp tương đương
* Xác định các ca kiểm thử

_**Nguyên tắc:**_

* 1 lớp các giá trị lớn hơn
* 1 lớp các giá trị nhỏ hơn
* n lớp các giá trị hợp lệ

_**Ví dụ**:_ Thiết kế testcase cho ô text chỉ cho nhập số nguyên với độ dài ký tự thuộc \[1-10] hoặc \[20-30]

_Với yêu cầu trên ta có các vùng:_

* nhỏ hơn 1 : vùng không hợp lệ
* \[1-10] : vùng hợp lệ
* lớn hơn 10 và nhỏ hơn 20 : vùng không hợp lệ
* \[20-30] : vùng hợp lệ
* lớn hơn 30: vùng không hợp lệ
* Nhập các ký tự không phải số nguyên : vùng không hợp lệ

_Vì vậy có các case:_

* Case hợp lệ:
  * Nhập 5 ký tự
  * Nhập 25 ký tự số
* Case không hợp lệ:
  * Không nhập vào trường
  * Nhập 15 ký tự
  * Nhập số thập phân
  * Nhập 35 kí tự
  * Nhập ký tự chữ: Tiếng việt, Tiếng anh, Full-size, Half-size
  * Nhập ký tự đặc biệt, space, kí tự Enter
  * Nhập câu lệnh SQL injection, HTML, XSS

### 5.2. Phân tích giá trị biên (Boundary Value Analysis (BVA) )

Phân tích giá trị biên dựa trên việc kiểm thử tại các ranh giới giữa các phân vùng, Chúng ta sẽ tập trung vào các giá trị biên chứ không test toàn bộ dữ liệu. Thay vì chọn nhiều giá trị trong lớp đương tương để làm đại diện, phân tích giá trị biên yêu cầu chọn một hoặc vài giá trị là các cạnh của lớp tương đương để làm điều kiện test.

Chúng ta thường thấy rằng một số lượng lớn lỗi xảy ra tại các ranh giới của các giá trị đầu vào được xác định thay vì các giá trị giữa, còn được gọi là các giá trị biên. Từ đó đưa ra lựa chọn các test cases thực hiện giá trị đầu vào các giá trị biên.

Kỹ thuật thiết kế test cases này bổ sung cho phân vùng tương đương. Kỹ thuật kiểm thử phần mềm này dựa trên nguyên tắc: Nếu một hệ thống hoạt động tốt với các giá trị biên thì nó sẽ hoạt động tốt cho tất cả các giá trị nằm giữa hai giá trị biên.

Phân tích giá trị biên sẽ chọn các giá trị:

* Giá trị ngay dưới giá trị nhỏ nhất
* Giá trị nhỏ nhất
* Giá trị ngay trên giá trị nhỏ nhất
* Giá trị ngay dưới giá trị lớn nhất
* Giá trị lớn nhất
* Giá trị ngay trên giá trị lớn nhất

**Ví dụ**: Với ví dụ trên ta có các case:

* Không nhập ký tự nào (Giá trị ngay dưới giá trị nhỏ nhất vùng 1)
* Nhập 1 ký tự (giá trị nhỏ nhất vùng 1)
* Nhập 2 ký tự (giá trị ngay trên giá trị nhỏ nhất vùng 1)
* Nhập 9 ký tự (giá trị ngay dưới giá trị lớn nhất vùng 1)
* Nhập 10 ký tự(giá trị lớn nhất vùng 1)
* Nhập 11 ký tự(giá trị ngay trên giá trị lớn nhất vùng 1)
* Nhập 19 ký tự (giá trị ngay dưới giá trị nhỏ nhất vùng 2)
* Nhập 20 ký tự(giá trị nhỏ nhất vùng 2)
* Nhập 21 ký tự (giá trị ngay trên giá trị nhỏ nhất vùng 2)
* Nhập 29 ký tự(giá trị ngay dưới giá trị lớn nhất vùng 2)
* Nhập 30 ký tự(giá trị lớn nhất vùng 2)
* Nhập 31 ký tự(giá trị ngay trên giá trị lớn nhất vùng 2)

**=>** Kết hợp kỹ thuật phân vùng tương đương với phân tích giá trị biên ta có các case:

* Không nhập ký tự nào
* Nhập 1 ký tự
* Nhập 5 ký tự
* Nhập 10 ký tự
* Nhập 11 ký tự
* Nhập 19 ký tự
* Nhập 20 ký tự
* Nhập 21 ký tự
* Nhập 25 ký tự
* Nhập 30 ký tự
* Nhập 31 ký tự
* Nhập số thập phân
* Nhập ký tự chữ: Tiếng việt, Tiếng anh, Full-size, Half-size
* Nhập ký tự đặc biệt, space, kí tự Enter
* Nhập câu lệnh SQL injection, HTML, XSS

### 5.3. Bảng quyết định (Decision Table based testing)

Bảng quyết định còn được gọi là bảng Nguyên nhân – Kết quả (Cause-Effect).

Kỹ thuật kiểm thử phần mềm này được sử dụng cho các chức năng cần sự kết hợp của các yếu tố đầu vào các biến.

**Ví dụ**: Nút Submit phải được enable nếu người dùng đã nhập tất cả các trường bắt buộc.

Đầu tiên là xác định đấu ra của các chức năng có phụ thuộc vào sự kết hợp của các đầu vào. Nếu có tập hợp kết hợp đầu vào lớn, thì hãy chia nó thành các tập hợp nhỏ hơn hữu ích cho việc quản lý bảng quyết định.

Đối với mọi chức năng, cần tạo một bảng và liệt kê tất cả các loại kết hợp đầu vào và đầu ra tương ứng. Điều này giúp xác định các điều kiện bị tester bỏ qua.

Các bước để tạo bảng quyết định:

* Nhập đầu vào theo hàng
* Nhập tất cả các quy tắc trong cột
* Điền vào bảng với sự kết hợp của đầu vào
* Trong hàng cuối cùng, ghi chú đầu ra so với kết hợp đầu vào.

**Ví dụ**: Nút **Submit** chỉ được enable khi tất cả các đầu vào được nhập bởi người dùng cuối.

![](<../.gitbook/assets/image (12).png>)
