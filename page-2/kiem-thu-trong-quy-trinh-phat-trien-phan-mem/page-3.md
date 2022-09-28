---
description: Duyenntm
---

# Test type

## 1. Test Type là gì?

**Test Type** có thể được hiểu là sự phân loại các hoạt động kiểm thử theo mục đích, chiến thuật kiểm thử. Mỗi Test Type sẽ gắn với một mục tiêu kiểm thử nhất định.

<figure><img src="../../.gitbook/assets/image (9) (6).png" alt=""><figcaption></figcaption></figure>

Trong kiểm thử phần mềm được chia thành 4 loại:

* **Functional Testing** (Kiểm thử chức năng)
* **Non-functional Testing** (Kiểm thử phi chức năng)
* **Structural Testing** (Kiểm thử cấu trúc)
* **Change-related Testing** (Kiểm thử thay đổi)

## 2. Các Test Type chính

### 2.1. Testing of function ( Functional testing)

**Kiểm thử chức năng** là kiểm tra xem hệ thống có hoạt động theo đúng theo các yêu cầu nghiệp vụ không? Kiểm thử chức năng được thực hiện ở tất cả các mức kiểm thử.

**Kiểm thử chức năng có thể được thực hiện từ 2 góc nhìn:**

_Dựa trên yêu cầu:_

* Sử dụng các đặc tả kỹ thuật của các yêu cầu chức năng để làm cơ sở cho việc test các thiết kế.
* Nội dung của các yêu cầu có thể làm các mục kiểm thử ban đầu hoặc sử dụng nó như là một danh sách các mục kiểm thử hoặc không kiểm thử.
* Dựa theo yêu cầu để phân mức độ ưu tiên trong quá trình kiểm thử. Cần ưu tiên các yêu cầu có mức độ rủi ro cao.

_Dựa trên quy trình nghiệp vụ:_

* Các quy trình nghiệp vụ mô tả các kịch bản scenarios liên quan đến các nghiệp vụ hằng ngày của hệ thống
* Các usecase được bắt nguồn phát triển theo hướng đối tượng nhưng hiện tại phổ biến trong nhiều trong các vòng đời phát triển.
* Lấy các quy trình nghiệp vụ làm điểm khởi đầu, các quy trình nghiệp vụ xuất phát từ các nhiệm vụ được thực hiện bởi người dùng.
* Các use case là một cơ sở hữu ích cho các testcase từ góc độ nghiệp vụ.

**Kiểm thử chức năng bao gồm 5 bước:**

* Xác định các chức năng mà phần mềm mong muốn sẽ thực hiện.
* Tạo các dữ liệu đầu vào dựa trên các tài liệu đặc tả kỹ thuật của các chức năng.
* Xác định các kết quả đầu ra dựa trên các tài liệu đặc tả kỹ thuật của các chức năng.
* Thực hiện các trường hợp kiêm thử.
* So sánh kết quả thực tế và kết quả mong muốn.

**Các loại kiểm thử chức năng bao gồm:**

* Kiểm thử đơn vị (Unit Testing)
* Smoke Testing
* Kiểm thử giao diện (Interface Testing)
* Kiểm thử tích hợp (Integration Testing)
* Kiểm thử hệ thống (System Testing)
* Kiểm thử hồi quy (Regression Testing)
* Kiểm thử chấp nhận (Acceptance Testing)

### 2.2. Testing of software product characteristics (Non - Functional testing)

Kiểm thử phi chức năng giống kiểm thử chức năng ở chỗ cả hai đều xuất hiện trong mọi mức độ kiểm thử.

Nếu như Functional Testing hướng tới việc test toàn thể chức năng hoặc một chức năng cụ thể thì Non-functional Testing được thực hiện nhằm trả lời câu hỏi: _“Phần mềm có hoạt động tốt không?”_.

Kiểm thử phi chức năng chú trọng nhiều hơn vào những khía cạnh khác của phần mềm, như là độ bảo mật và khả năng tải của phần mềm đó, ví dụ như bao nhiêu người có thể đăng nhập cùng 1 lúc.

**Kiểm thử phi chức năng bao gồm:**

* Kiểm thử hiệu năng (Performance testing)
* Kiểm thử khả năng chịu tải (Load testing)
* Kiểm thử áp lực (Stress testing)
* Kiểm thử tính khả dụng (Usability testing)
* Kiểm thử bảo trì (Maintainability testing)
* Kiểm thử độ tin cậy (Reliability testing)
* Kiểm thử tính tương thích (Portability testing)

**Các đặc điểm và các đặc điểm phụ tương ứng:**

* **Chức năng** (Functionality) gồm 5 đặc điểm phụ: sự phù hợp, chính xác, bảo mật, khả năng tương tác và tuân thủ.
* **Độ tin cậy** (Reliability) gồm 4 đặc điểm phụ: độ bền, khả năng chịu lỗi, khả năng phục hồi và tuân thủ.
* **Khả năng sử dụng** (Usability) gồm 5 đặc điểm phụ: dễ hiểu, khả năng học hỏi, khả năng hoạt động, sự thu hút và tính tuân thủ.
* **Tính hiệu quả** (Efficiency) gồm 3 đặc điểm phụ: thời gia (hiệu suất), sử dụng tài nguyên và tuân thủ.
* **Khả năng bảo trì** (Maintainability) gồm 5 đặc điểm phụ: khả năng phân tích, khả năng thay đổi, tính ổn định, khả năng kiểm tra và tuân thủ.
* **Tính tương thích** (Portability) gồm 5 đặc điểm phụ: khả năng thích ứng, khả năng cài đặt, cùng tồn tại, khả thăng thay thế và tuân thủ.

### 2.3. Testing of software structure/architecture ( Structural testing)

* Kiểm thử cấu trúc thường được gọi là "hộp trắng" hoặc "hộp thủy tinh" vì chúng quan tâm đến những gì đang xảy ra bên trong hộp.
* Kiểm thử cấu trúc thường được sử dụng như một cách đo lường của kiểm thử thông qua độ bao phủ của một tập hợp các yếu tố cấu trúc hoặc các mục bao phủ.
* Nó có thể xảy ra ở bất kỳ mức độ kiểm thử nào chủ yếu ở kiểm thử thành phần, tích hợp.
* Ở cấp độ thành phần, và mức thấp hơn trong kiểm thử tích hợp thành phần có hỗ trợ công cụ tốt để đo mức độ bao phủ của mã. Các công cụ đo lường độ bao phủ đánh giá tỉ lệ phần trăm thực thi đã được thực hiện bởi một bộ kiểm thử. Nếu độ bao phủ không phải là 100% thì các kiểm thử bổ sung có thể cần phải được viết và chạy để bao phủ những phần chưa được thực hiện.
* Các kỹ thuật được sử dụng để kiểm tra cấu trúc là kỹ thuật kiểm thử hộp trắng, các mô hình luồng điều khiển thường sử dụng để hỗ trợ kiểm thử cấu trúc.

### 2.4. Testing related to changes (Confirmation and regression testing)

Mục đích của kiểm thử thay đổi là để kiểm tra xem phần mềm có vận hành trơn tru sau những lần sửa lỗi hay không.

Kiểm thử thay đổi gồm 2 loại chính:

* **Confirmation Testing** (Kiểm thử xác nhận): Thường Confirmation Testing sẽ diễn ra sau khi lỗi trong phần mềm đã được xác nhận và được sửa. Lúc này, vai trò của Kiểm thử xác nhận là để xem lỗi đã thực sự được sửa hay chưa. Các tester sẽ tiến hành bằng cách cho một input giống hệt ban đầu và test xem output có ra được như mong muốn hay không.
* **Regression Testing** (Kiểm thử hồi quy): Mục đích của kiểm thử hồi quy để xác nhận rằng các thay đổi trong phần mềm hoặc môi trường không gây ra bất lợi ngoài mong muốn và hệ thống vẫn đáp ứng các yêu cầu. Kiểm thử hồi quy được thực hiện khi phần mềm thay đổi, do sửa lỗi hoặc do chức năng mới. Việc thực thi Regression Testing cũng nên được cân nhắc khi môi trường xung quanh phần mềm có sự thay đổi.
