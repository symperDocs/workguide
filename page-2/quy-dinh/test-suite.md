---
description: Thanhntp
---

# Test Suites

## **Nội dung đối tượng**

**Test Suite:** là tập hợp của các Test Cases (trường hợp kiểm thử) nhằm mục đích để kiểm tra một chương trình phần mềm. Khi có các trường hợp kiểm thử, bạn sẽ cần phân loại các trường hợp theo từng tình huống kiểm thử khác nhau, như kiểm thử chức năng hoặc cho các tính năng riêng biệt của phần mềm.

## **Đặc điểm của đối tượng**

Thông thường, một Test Suites sẽ có một vài đặc điểm chính sau:

* Test Suites được tạo ra sau Test Plan (kế hoạch kiểm thử).
* Test Suites bao gồm các trường hợp kiểm thử.
* Miêu tả mục tiêu và kết quả mong muốn của các trường hợp kiểm thử.
* Test Suites bao gồm các thông số kiểm thử, như ứng dụng, môi trường, phiên bản, v.v…
* Bao gồm nhiều kiểu kiểm thử, như kiểm thử chức năng hoặc phi chức năng.
* Giúp tăng hiệu suất của quá trình kiểm thử bằng cách kiểm thử liên tục và cải thiện phần mềm đang được test.
* Có thể được sử dụng bởi nhiều công cụ tự động như jUnit, Selenium, etc.

## **Quy định và khung đánh giá**

### **Quy định thiết kế Test Suites**

Test Suites là tập hợp các Test Case. Test case **** là một trong những yếu tố ảnh hưởng đến chi phí test. Số lượng test case càng nhiều thì quá trình kiểm thử sẽ càng tốn nhiều thời gian và tiền bạc. Ngoài ra, tuy số lượng test case nhiều, nhưng nếu các test case không chính xác thì tất cả sẽ như “bỏ đi”. Chất lượng sản phẩm sẽ không được đảm bảo.

Do đó, phải thiết kế test case thật tối ưu và hiệu quả trước khi bắt đầu kiểm thử. Nhưng làm sao để thiết kế test case tối ưu nhất? Đó chính là sử dụng các kỹ thuật test và các phương pháp test.

Test Suites được tạo ra sau Test Plan nên khi Test Plan tạo và được duyệt mới có thể tạo Test Suites.&#x20;

Bắt buộc tạo Test Suites bằng quy trình trong Application. Nghiêm cấm import dữ liệu.

Quy định số lượng Test cases trong mỗi Test Suites: max: 500 Test Case, min: 50 Test Case.

**Lưu ý khi viết Test Cases**:

* File Test Case cần có những bước test đơn giản, minh bạch, dễ hiểu.
* Bước test phải viết chi tiết rõ ràng để ngay cả khi QC khác đọc có thể thực hiện được.
* Mục đích và phạm vi của Test Case cũng được mô tả chi tiết.
* Điều kiện tiền đề, data test cũng phải được ghi ở từng Test Case nếu cần.
* Test Case nên được review chéo bởi member trong team.
* Không nên gộp quá nhiều kết quả confirm vào 1 case mà nên tách mỗi kết quả confirm ra từng case.
* Khi tạo Test Case nên đứng ở vị trí End user.

### **Khung đánh giá Test Suites**

**Một testcase hiệu quả cần có các đặc điểm sau:**

* Chính xác, đầy đủ nghiệp vụ hệ thống**.**
* Độc lập (có thể thực hiện mà không phụ thuộc vào các Test Case khác, dễ dàng chia cho nhiều người cùng kiểm thử).
* Nội dung đơn giản, có mục đích rõ ràng và ai đọc cũng hiểu theo một cách duy nhất. (đầu vào, đầu ra, các bước thực hiện rõ ràng)
* Trình bày mạch lạc thống nhất cho toàn bộ tài liệu.
* Có khả năng tái sử dụng (có thể dễ dàng cập nhật và sửa đổi).

****





****
