---
description: Duyenntm
---

# Kiểm thử hộp trắng

## 1. Kiểm thử hộp trắng là gì?

_**Kỹ thuật kiểm thử hộp trắng**_ (còn được gọi là kỹ thuật dựa trên cấu trúc hoặc cấu trúc) dựa trên phân tích kiến trúc, thiết kế chi tiết, cấu trúc bên trong hoặc mã của đối tượng kiểm tra. Không giống như kỹ thuật kiểm thử hộp đen, kỹ thuật kiểm thử hộp trắng tập trung vào cấu trúc và quá trình xử lý bên trong đối tượng kiểm thử.

Người kiểm tra chọn đầu vào để thực hiện các đường dẫn thông qua mã và xác định đầu ra thích hợp. Kiến thức lập trình và kiến thức thực hiện là rất cần thiết trong kiểm thử hộp trắng.

![](<../.gitbook/assets/image (18).png>)

_**Kiểm thử hộp trắng để kiểm thử:**_

* Các lệnh trong chương trình
* Các điều kiện logic&#x20;
* Các chu trình lặp lại&#x20;
* Cấu trúc dữ liệu&#x20;
* Các luồng điều khiển

## 2. Mức độ áp dụng

Phương pháp Kiểm thử hộp trắng áp dụng cho các mức độ kiểm thử phần mềm sau đây:

* Unit Testing(Kiểm thử đơn vị): Để kiểm tra đường dẫn trong một đơn vị.
* Integration Testing(Test tích hợp): Để kiểm tra đường dẫn giữa các đơn vị.
* System Testing(Test hệ thống): Để kiểm tra các đường dẫn giữa các hệ thống con.

Tuy nhiên, nó là chủ yếu áp dụng cho các kiểm thử đơn vị .

## 3. Ưu điểm và nhược điểm của kiểm thử hộp trắng

**Ưu điểm:**

* Test có thể bắt đầu ở giai đoạn sớm hơn, không cần phải chờ đợi cho GUI để có thể test
* Test kỹ càng hơn, có thể bao phủ hầu hết các đường dẫn
* Thích hợp trong việc tìm kiếm lỗi và các vấn đề trong mã lệnh
* Cho phép tìm kiếm các lỗi ẩn bên trong
* Các lập trình viên có thể tự kiểm tra
* Giúp tối ưu việc mã hoá
* Do yêu cầu kiến thức cấu trúc bên trong của phần mềm, nên việc kiểm soát lỗi tối đa nhất.

**Nhược điểm:**

* Vì các bài kiểm tra rất phức tạp, đòi hỏi phải có các nguồn lực có tay nghề cao, với kiến thức sâu rộng về lập trình và thực hiện.
* Maintenance test script có thể là một gánh nặng nếu thể hiện thay đổi quá thường xuyên.
* Vì phương pháp thử nghiệm này liên quan chặt chẽ với ứng dụng đang được test, nên các công cụ để phục vụ cho mọi loại triển khai / nền tảng có thể không sẵn có.

## **4.** Các kỹ thuật kiểm thử hộp trắng phổ biến

### 4.1 Kiểm tra tuyên bố và phạm vi bảo hiểm

Kiểm tra câu lệnh thực hiện các câu lệnh thực thi tiềm năng trong mã. Mức độ phù hợp được đo bằng số câu lệnh được thực thi bởi các thử nghiệm chia cho tổng số câu lệnh có thể thực thi trong đối tượng thử nghiệm, thường được biểu thị bằng phần trăm.

### 4.2 Kiểm tra quyết định và phạm vi bảo hiểm

Kiểm tra quyết định thực hiện các quyết định trong mã và kiểm tra mã được thực thi dựa trên kết quả quyết định. Để thực hiện điều này, các trường hợp thử nghiệm tuân theo các luồng kiểm soát xảy ra từ một điểm quyết định (ví dụ: đối với câu lệnh IF, một trường hợp cho kết quả đúng và một trường hợp cho kết quả sai; đối với câu lệnh CASE, các trường hợp thử nghiệm sẽ được yêu cầu cho tất cả các kết quả có thể xảy ra, bao gồm cả kết quả mặc định).

Mức độ phù hợp được đo bằng số lượng kết quả quyết định được thực hiện bởi các thử nghiệm chia cho tổng số kết quả quyết định trong đối tượng thử nghiệm, thường được biểu thị bằng phần trăm.

### 4.3 Giá trị của Tuyên bố và Kiểm tra Quyết định

Khi đạt được mức độ bao phủ câu lệnh 100%, nó đảm bảo rằng tất cả các câu lệnh thực thi trong mã đã được kiểm tra ít nhất một lần, nhưng nó không đảm bảo rằng tất cả logic quyết định đã được kiểm tra. Trong số hai kỹ thuật hộp trắng được thảo luận trong giáo trình này, kiểm tra tuyên bố có thể cung cấp ít phạm vi hơn kiểm tra quyết định.

Khi đạt được mức độ bao phủ quyết định 100%, nó thực hiện tất cả các kết quả quyết định, bao gồm cả việc kiểm tra kết quả đúng và cả kết quả sai, ngay cả khi không có tuyên bố sai rõ ràng (ví dụ: trong trường hợp câu lệnh IF mà không có câu lệnh khác trong mã). Mức độ bao phủ của tuyên bố giúp tìm ra các khiếm khuyết trong mã chưa được thực hiện bởi các thử nghiệm khác. Phạm vi quyết định giúp tìm ra các khiếm khuyết trong mã mà các thử nghiệm khác không thực hiện được cả kết quả đúng và sai.

Việc đạt được mức độ bao phủ quyết định 100% đảm bảo mức độ bao phủ của câu lệnh là 100% (nhưng không phải ngược lại).
