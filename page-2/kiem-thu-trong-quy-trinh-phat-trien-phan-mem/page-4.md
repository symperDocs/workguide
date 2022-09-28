# Test level

<figure><img src="../../.gitbook/assets/image (10) (3).png" alt=""><figcaption></figcaption></figure>

* Tách riêng từng phần để kiểm tra và chứng minh các thành phần đó thực hiện chính xác các yêu cầu chức năng trong đặc tả.
* Lỗi được sửa sớm trong chu trình phát triển phần mềm vì vậy tiết kiệm thời gian và chi phí sửa lỗi.
* Mã nguồn được tái sử dụng nhiều hơn.
* Tăng sự tin tưởng trong việc thay đổi hoặc bảo trì
* Mã nguồn đáng tin cậy hơn.

### **1.3. Phương pháp**

Sử dụng phương pháp Kiểm thử hộp trắng

### **1.4. Người thực hiện**

Thường là developer thực hiện

## 2. Integration Test - Kiểm thử tích hợp

### **2.1. Khái niệm**

**Kiểm thử tích hợp** là loại kiểm thử trong đó các module phần mềm hay từng chức năng riêng lẻ được tích hợp logic và được kiểm tra theo nhóm. Mỗi dự án phần mềm gồm nhiều modules, được code bởi nhiều người khác nhau, vì vậy kiểm thử tích hợp tập chung vào việc kiểm tra truyền dữ liệu giữa các module.

**Ví dụ:** Có 2 module Login, Tạo tài khoản cho người dùng

* Admin tạo tài khoản cho người dùng thành công, tài khoản có trạng thái là đang hoạt động. Người dùng sử dụng tài khoản vừa tạo đăng nhập thành công vào hệ thống.
* Nếu Admin chuyển tài khoản này thành trạng thái ngừng hoạt động. Người dùng sử dụng tài khoản này đăng nhập, hệ thống sẽ báo không thành công.

### **2.2. Mục đích**

* Phát hiện lỗi tương tác xảy ra giữa các Unit.
* Tập chung chủ yếu vào các giao diện và thông tin giữa các module.
* Tích hợp các Unit đơn lẻ thành các hệ thống nhỏ.

### **2.3. Cách tiếp cận/ phương pháp**

#### **2.3.1. Big Bang**

Theo cách này, tất cả các thành phần được tích hợp với nhau cùng một lúc và sau đó được kiểm thử.

<figure><img src="../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>

**Ưu điểm:**

* Thuận tiện cho các hệ thống nhỏ.

**Nhược điểm:**

* Kiểm tra lỗi nội địa hóa (Localization) là một thử thách.
* Có nhiều lỗi về giao diện cần được kiểm thử theo phương pháp này, một số liên kết giao diện cần kiểm thử có thể dễ dàng bị bỏ qua.
* Kiểm thử Tích hợp chỉ có thể bắt đầu sau khi "tất cả" các mô-đun được thiết kế, nên nhóm thử nghiệm sẽ có ít thời gian thực hiện hơn trong giai đoạn thử nghiệm.
* Vì tất cả các mô-đun được kiểm tra cùng một lúc, các mô-đun quan trọng có rủi ro cao không được ưu tiên hay kiểm tra riêng. Các mô-đun ngoại vi liên quan đến giao diện người dùng cũng không được ưu tiên hay kiểm tra riêng.

#### **2.3.2. Top Down**

Trong Phương pháp Top Down, việc kiểm thử diễn ra từ trên xuống dưới theo luồng điều khiển của hệ thống phần mềm. Lúc này, sẽ cần tới sự hỗ trợ của Stubs trong việc kiểm thử.

<figure><img src="../../.gitbook/assets/image (17) (6).png" alt=""><figcaption></figcaption></figure>

**Ưu điểm**

* Việc tìm kiếm bug trong từng module riêng biệt trở nên dễ dàng hơn
* Xây dựng một bản mẫu (prototype) ngay từ ban đầu là có thể
* Các mô-đun quan trọng được kiểm thử ưu tiên; lỗi thiết kế chính có thể được tìm thấy và sửa chữa trước

**Nhược điểm**

* Cần nhiều Stubs.
* Các mô-đun ở mức thấp hơn được kiểm thử không đầy đủ.

#### **2.3.3. Bottom up**

Trong Phương pháp Bottom up, mỗi mô-đun ở các cấp thấp hơn được kiểm tra với các mô-đun cao hơn cho đến khi tất cả các mô-đun được kiểm tra. Lúc này, sẽ cần tới sự hỗ trợ của Driver trong việc kiểm thử.

<figure><img src="../../.gitbook/assets/image (2) (2).png" alt=""><figcaption></figcaption></figure>

* Các mô-đun quan trọng (ở cấp cao nhất của kiến trúc phần mềm) mà kiểm soát luồng ứng dụng được kiểm tra cuối cùng và có thể dễ bị lỗi.
* Xây dựng một bản mẫu (prototype) ngay từ ban đầu - là một điều không thể

#### **2.3.4. Sandwich/Hybrid**

Phương pháp sandwich / hybrid là sự kết hợp của phương pháp Top Down và bottom up. Ở đây, các mô-đun hàng đầu được kiểm tra với các mô-đun thấp hơn đồng thời các mô-đun thấp hơn được tích hợp với các mô-đun hàng đầu và được kiểm thử. Chiến lược này sử dụng cả Stubs cũng như Drivers.

* Các mô-đun quan trọng (ở cấp cao nhất của kiến trúc phần mềm) mà kiểm soát luồng ứng dụng được kiểm tra cuối cùng và có thể dễ bị lỗi.
* Xây dựng một bản mẫu (prototype) ngay từ ban đầu - là một điều không thể

#### **2.3.4. Sandwich/Hybrid**

Phương pháp sandwich / hybrid là sự kết hợp của phương pháp Top Down và bottom up. Ở đây, các mô-đun hàng đầu được kiểm tra với các mô-đun thấp hơn đồng thời các mô-đun thấp hơn được tích hợp với các mô-đun hàng đầu và được kiểm thử. Chiến lược này sử dụng cả Stubs cũng như Drivers.

<figure><img src="../../.gitbook/assets/image (19) (2).png" alt=""><figcaption></figcaption></figure>

###

### 2.4. **Người thực hiện**

Thường là Tester thực hiện

## 3. System Test - Kiểm thử hệ thống

### **3.1. Khái niệm**

**Kiểm thử hệ thống** là kiểm thử toàn bộ chức năng và giao diện của hệ thống.

### **3.2. Mục đích**

Đánh giá hệ thống có đáp ứng theo đúng yêu cầu nghiệp vụ, yêu cầu về chức năng đưa ra hay không.

### **3.4. Phân loại**

Dưới đây là một số loại kiểm thử thường được thực hiện trong System Test:

* Kiểm thử chức năng (Functional Test): Là kiểm thử toàn bộ hệ thống, đảm bảo hệ thống hoạt động đúng theo yêu cầu được đưa ra trước đó.
* Kiểm thử hiệu năng (Performance Test): Là kiểm tra sự tuân thủ của hệ thống với các yêu cầu được chỉ định về hiệu năng. Xác định những thuộc tính chất lượng của hệ thống như khả năng mở rộng, độ tin cậy...
* Kiểm thử cơ sở dữ liệu ( Database Test): Là kiểm tra dữ liệu hiển thị trên hệ thống có giống với dữ liệu trong cơ sở dữ liệu hay không?
* Kiểm thử khả năng bảo mật ( Security Test): Là kiểm tra hệ thống được bảo vệ an toàn, không bị đánh cắp dữ liệu, thông tin trước các tấn công từ bên ngoài.
* Kiểm thử tính khả dụng (Usability Test): Kiểm tra tính thân thiện với người dùng và tính dễ sử dụng của hệ thống.
* Kiểm tra tính tương thích ( Compatibility Test) : Là kiểm tra xem hệ thống có tương thích với các yếu tố khác của hệ thống mà nó sẽ hoạt động hay không? (Ví dụ: Trình duyệt, hệ điều hành, phần cứng)
* Kiểm tra khả năng phục hồi ( Recovery Test): Là kiểm tra hệ thống có khả năng khôi phục trạng thái ổn định khi gặp các sự cố bất thường không

### **3.5. Phương pháp**

Kiểm thử hộp đen là phổ biến

### **3.6. Người thực hiện**

Thường là Tester thực hiện

## 4. Acceptance Test - Kiểm thử chấp nhận

### **4.1. Khái niệm**

**Kiểm thử chấp nhận** là kiểm tra xem phần mềm đã thỏa mãn tất cả yêu cầu của khách hàng chưa? Và khách hàng có chấp nhận sản phẩm hay không?

### **4.2. Mục đích**

Để nghiệm thu hệ thống trước khi hệ thống được đưa vào hoạt động.

### **4.3. Phân loại**

Trong kiểm thử chấp nhận lại chia ra làm 2 loại:

* **Alpha test:** Được thực hiện bởi các thành viên của tổ chức phát triển phần mềm nhưng không liên quan trực tiếp đến dự án (Thường là các thành viên của quản lý sản phẩm). Alpha test thực hiện test tại nơi sản xuất phần mềm, là một hình thức kiểm thử nội bộ, trước khi phần mềm được tiến hành kiểm thử Beta.
* **Beta test:** Được thực hiện bởi người dùng cuối cùng (thường là khách hàng). Beta test thực hiện tại địa điểm của khách hàng, người dùng test hay sử dụng hệ thống trong môi trường riêng của họ - không phải nơi phát triển phần mềm.

### **4.4. Phương pháp**

Kiểm thử hộp đen

### **4.5. Người thực hiện**

Khách hàng hoặc bên thứ 3
