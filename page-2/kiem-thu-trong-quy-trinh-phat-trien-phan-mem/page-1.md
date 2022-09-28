---
description: Duyenntm
---

# Maintenance Testing

## 1. Khái niệm

**Kiểm thử bảo trì** là kiểm tra những thay đổi tới hoạt động hệ thống hoặc tác động của thay đổi môi trường tới hoạt động hệ thống.

Thông thường kiểm thử bảo trì gồm 2 phần: kiểm thử các thay đổi và Kiểm thử hồi quy để cho thấy phần còn lại của hệ thống không bị ảnh hưởng bởi công việc bảo trì.&#x20;

Hoạt động chính và quan trọng trong việc kiểm thử bảo trì là việc phân tích các tác động. Từ việc phân tích sẽ quyết định được những phần nào của hệ thống có thể bị ảnh hưởng không mong muốn. Phân tích rủi ro sẽ giúp quyết định được nơi cần tập trung kiểm thử hồi quy.

## **2. Khởi động cho kiểm thử bảo trì:**

* Sau khi triển khai, một hệ thống phần mềm thường được phục vụ trong nhiều năm hoặc nhiều thập kỷ. Trong thời gian này cấu hình dữ liệu hoặc môi trường của hệ thống thường được sửa chữa, thay đổi và mở rộng. Việc lập kế hoạch của các phiên bản phát hành trước đó là quan trọng cho kiểm thử bảo trì thành công.
* Kiểm thử bảo trì được thực hiện trên hệ thống đã tồn tại, và được thực hiện khi có sự thay đổi, di chuyển hoặc rút lui của phần mềm hoặc hệ thống.
* Kiểm thử bảo trì cho việc thay đổi : Bao gồm việc lập kế hoạch cải tiến thay đổi như là lập kế hoạch nâng cấp cơ sở dữ liệu, hệ điều hành.
* Kiểm thử bảo trì cho việc di chuyển : Bao gồm kiểm tra hoạt động của môi trường mới , các phần mềm đã thay đổi. Kiểm thử di chuyển ( kiểm thử chuyển đổi) cũng cần thiết khi dữ liệu từ một ứng dụng khác sẽ được di chuyển vào hệ thống đang được bảo trì.
* Kiểm thử bảo trì cho việc rút lui của một hệ thống : Bao gồm kiểm thử chuyển đổi dữ liệu hoặc lưu trữ dữ liệu
* Kiểm thử bảo trì bao gồm kiểm thử hồi quy đến các bộ phận thay đổi của hệ thống .
* Phạm vi của kiểm thử bảo trì liên quan đến rủi ro của việc thay đổi , kích thước của hệ thống hiện có, và kích thước của sự thay đổi
* Kiểm thử bảo trì được thực hiện tại bất kỳ hoặc tất cả các mức độ kiểm thử hoặc tất cả các loại kiểm thử .
* Kiểm thử bảo trì có thể khó khăn nếu đặc điểm kỹ thuật lỗi thời hoặc biến mất hoặc người kiểm thử không có sẵn các kiển thức về miền (domain).
