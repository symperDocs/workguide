---
description: Duyenntm
---

# Test Plan

## Định nghĩa

**Test plan** chính là tài liệu tổng quan về việc kiểm thử 1 project đặc tả: phạm vi dự án, hướng tiếp cận, quy trình kiểm thử, tài nguyên và nhân lực cần có, các tính năng cần được test và không cần phải test, các công cụ và môi trường test cần có. Test plan giúp tester xác định nỗ lực cần thiết để xác nhận chất lượng của ứng dụng đang được kiểm thử phần mềm.

## Tầm quan trọng của Test Plan

* Giúp những người ngoài nhóm kiểm thử như nhà phát triển, quản lý doanh nghiệp, khách hàng hiểu chi tiết về kiểm thử.
* Test plan hướng dẫn suy nghĩ của chúng ta. Nó giống như một cuốn sách quy tắc, cần phải được tuân theo.
* Các khía cạnh quan trọng như ước tính kiểm thử, phạm vi kiểm thử, chiến lược kiểm thử được ghi lại trong test plan. Do đó, nhóm quản lý có thể xem xét và sử dụng lại cho các dự án khác.

## Các bước tạo nên Test Plan

Như các bạn đã biết lập **Test Plan** là nhiệm vụ quan trọng nhất của quy trình quản lý kiểm thử. Dưới đây là 8 bước để tạo ra một Test Plan hoàn chỉnh.

#### Bước 1. Phân tích sản phẩm

Đây là bước đầu tiên cực kỳ quan trọng đối với bất kỳ một quá trình kiểm thử nào. Bạn cần đặt ra những câu hỏi cơ bản nhất xoay quanh sản phẩm và đi tìm câu trả lời. Chẳng hạn như:

* Đối tượng sử dụng là ai?
* Mục đích sử dụng là gì?
* Cần có những phần mềm hay phần cứng nào?

Nghiên cứu và phân tích sản phẩm sẽ hạn chế được tối thiểu những sai lầm không đáng có sau này.

#### Bước 2. Xây dựng chiến lược kiểm thử

Chiến lược kiểm thử sẽ chi tiết hóa những nội dung như:

* Phạm vi test ra sao?
* Phần nào sẽ được test và phần nào không được test?
* Những hình thức test nào cần sử dụng?
* Những rủi ro và vấn đề nào có thể phát sinh trong quá trình test?

#### Bước 3. Xác định mục tiêu kiểm thử

Mỗi quá trình test sẽ có một mục tiêu khác nhau. Đó có có thể là tìm ra lỗi của phần mềm để tiếp tục phát triển, hay xác nhận phần mềm đã đủ tiêu chuẩn để đưa ra thị trường chưa. Do đó, xác định đúng mục tiêu sẽ giúp cho việc test sản phẩm diễn ra được nhanh chóng và suôn sẻ hơn.

#### Bước 4. Xác định tiêu chí kiểm thử

Tiêu chí kiểm thử (Test Criteria) bao gồm hai loại chính là:

* Tiêu chí tạm dừng (Suspension Criteria): nếu không thỏa mãn các tiêu chí này thì quá trình test phải dừng lại. Ví dụ, nếu báo cáo cho thấy 40% trường hợp test thất bại, thì sẽ không tiếp tục quá trình test nữa. Nhóm test phải chuyển kết quả sang cho nhóm phát triển để khắc phục tất cả các lỗi hiện có.
* Tiêu chí thoát (Exit Criteria): là những điều kiện cần phải đạt được để có thể kết thúc quá trình test. Ví dụ, phần mềm được xem là phù hợp để đưa ra sử dụng nếu có 80% các trường hợp test thành công.

#### Bước 5: Lập kế hoạch về nguồn lực

Nguồn lực hay là các tài nguyên cho dự án test cũng là một vấn đề quan trọng. Nguồn lực có thể bao gồm nhiều yếu tố khác nhau. Đó có thể là con người, các thiết bị và vật liệu cần thiết để hoàn thành dự án. Điều này giúp người quản lý quá trình test có thể đưa ra một lịch trình phù hợp và ước lượng thời gian chính xác nhất để chạy dự án.

#### Bước 6: Xác định môi trường kiểm thử

Môi trường kiểm thử là tổng hợp tất cả những phần cứng và phần mềm mà cả team sẽ sử dụng. Kết quả của test plan sẽ phụ thuộc rất lớn vào các yếu tố thuộc về môi trường kiểm thử. Môi trường test lý tưởng nhất khi cho phép tester giám sát mọi biến động của phần mềm trong điều kiện sử dụng thực tế.

#### Bước 7: Sắp xếp lịch hoạt động

Ở bước tiếp theo, bạn cần phải lên kế hoạch thực sự cho dự án. Bạn có thể chia cả quá trình thành những task (nhiệm vụ) nhỏ. Từ đó có thể dễ dàng phân bổ thời gian và nhiệm vụ chi tiết cho mỗi task.

#### Bước 8: Kiểm soát sản phẩm thử nghiệm

Trong suốt quá trình test, bạn cần phải lập dữ liệu test, ghi lại nhật ký test. Sau khi test xong, bạn cần đưa ra được kết quả quá trình test. Bên cạnh đó là những báo cáo lỗi, cũng như là ghi chú về việc phát hành (release notes).

## **Hướng dẫn nhập liệu doc Test Plan (ID: 2847)**

### **Form nhập liệu doc và ý nghĩa từng thông tin trong doc**

![Test plan template](<../../.gitbook/assets/Screen Shot 2022-03-14 at 15.29.21.png>)

{% embed url="https://app.gitbook.com/s/-Mf66kQb8ODpdujUHM5j/format-tai-lieu-so-hoa-quy-trinh-noi-bo/8.4.-symper-test-plan" %}

### Cách sử dụng:&#x20;

**Bước 1:** Vào _**Ứng dụng của tôi**_** ** (1) trên hệ thống của Symper. Tại Sidebar hiển thị các ứng dụng chọn _**Quality Control**_** ** (2)**.** Tại sidebar chi tiết ứng dụng tìm kiếm quy trình _**SYMPER TEST PLAN**_ sau đó chuột phải chọn _**Bắt đầu**_ (3).

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 16.09.58.png>)

**Bước 2:** Tại form nhập liệu nhập giá trị cho các trường thông tin trong doc

![Form nhập liệu doc Test Plan](<../../.gitbook/assets/Screen Shot 2022-03-14 at 22.40.30.png>)

**Note:** Các trường require cần phải nhập

* STT: Nhập STT để tự động sinh ra Sub test plan ID.
* Sub SRS ID: Có thể tìm kiếm sub requirement tại cột Sub SRS ID. Khi chọn được Sub SRS ID sẽ tự động sinh ra SRS ID, Module, Module name, Sub module, Sub module name, Description.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.07.23.png>)

* Test environment: Lựa chọn môi trường test. Tại đây có thể lựa chọn nhiều môi trường test cùng lúc.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.06.11.png>)

* Test suite creator: Chọn người viết test case.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.05.38.png>)

* Tester: Chọn người kiểm thử (tương tự như chọn người viết test case) để chọn người thực hiện kiểm thử.

**Bước 3:** Sau khi nhập đủ các trường thông tin trong doc thì nhấn nút gửi (1). Sau đó click button Hành động (2).

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.09.17 (1).png>)

Sau khi click button _**Hành động**_ sẽ hiển thị popup _**Hoàn thành công việc**_ thì click chọn _**Áp dụng**_

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.08.46.png>)
