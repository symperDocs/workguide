---
description: Duyenntm
---

# Test Run

Test run là gì?

Mục đích để làm gì?

Ý nghĩa các trường thông tin trong doc test run?

Tham khảo tại:

{% embed url="https://app.gitbook.com/s/-Mf66kQb8ODpdujUHM5j/format-tai-lieu-so-hoa-quy-trinh-noi-bo/8.11.-symper-test-run" %}

## **Hướng dẫn nhập liệu doc Test Run (ID: 2368)**

**Bước 1:** Vào _**Ứng dụng của tôi**_** ** (1) trên hệ thống của Symper. Tại Sidebar hiển thị các ứng dụng chọn _**Quality Control**_** ** (2)**.** Tại sidebar chi tiết ứng dụng tìm kiếm quy trình _**SYMPER TEST RUN**_ sau đó chuột phải chọn _**Bắt đầu**_ (3).

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.35.15.png>)

**Bước 2:** Nhập dữ liệu

![Form nhập liệu](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.39.39.png>)

* Tại trường Test suites id nhập dữ liệu tìm kiếm để chọn id test suites. Sau khi chọn trường Test suites id sẽ tự động sinh ra id test run tại trường Test run id.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.40.17.png>)

* Tại trường Test method chọn phương thức thực hiện test

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.40.57 (1).png>)

* Sau khi chọn Test suites id, tại trường Test case id khi click vào sẽ hiển thị form bảng các test case nằm trong test suites đã chọn. Tích các test case muốn test sau đó nhân nút Lưu.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.41.36 (1).png>)

* Sau khi chọn các test case cần test thì sẽ hiển thị ID các test case đã chọn ở bảng bên dưới kèm theo các thông tin: Req ID, Sub req ID, Test case ID, Description, Test steps, Expect Result, Input data (nếu có) và trường Result mặc định là NEW.
* Tại đây, bạn cần nhập STT để doc tự động sinh ra Sub test run ID.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.48.00 (1).png>)

* Bạn cần đổi trạng thái các test case tại trường _**Result**_ để ghi nhận khoảng thời gian mỗi lần bạn thực hiện test một test case.

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.50.00 (1).png>)

* Trạng thái của test case được đổi từ _**NEW**_ sang _**PENDING**_ để ghi nhận thời gian bắt đầu test, khi đó trường _**Start date**_ sẽ ghi nhận ngày và hời gian bắt đầu test của bạn.
* Trạng thái test case đổi từ _**PENDING**_ sang _**PASS**_ hoặc _**FAILED**_ thì cột _**End date**_ sẽ ghi nhận thời gian kết thúc kiểm thử test case đó của bạn.
* Trong trường hợp khi trạng thái test case đó là _**FAILED**_ thì bạn cần nhập kết quả thực tế failed của case đó tại cột _**Actual result.**_

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.52.13.png>)

**Bước 3:** Sau khi nhập đủ các trường thông tin trong doc thì nhấn nút gửi (1). Sau đó click button Hành động (2).

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.53.21.png>)

Sau khi click button _**Hành động**_ sẽ hiển thị popup _**Hoàn thành công việc**_ thì click chọn _**Áp dụng**_

![](<../../.gitbook/assets/Screen Shot 2022-03-14 at 23.54.31.png>)
