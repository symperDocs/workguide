---
description: Duyenntm
---

# Kiểm thử dựa trên kinh nghiệm

## 1. Đoán lỗi(Error guessing) <a href="#21-c4-91o-c3-a1n-l-e1-bb-97ierror-guessing" id="21-c4-91o-c3-a1n-l-e1-bb-97ierror-guessing"></a>

Đoán lỗi là một phương pháp kiểm thử, trong đó các trường hợp kiểm thử được sử dụng để tìm lỗi trong các phần mềm dựa vào kinh nghiệm trong các lần kiểm thử trước của người kiểm thử (tester). Việc đoán lỗi thành công phụ thuộc rất nhiều vào kỹ năng của người kiểm thử, một người kiểm thử giỏi có thể biết được nơi nào có nhiều lỗi tiềm ẩn.

Đoán lỗi không có quy tắc rõ ràng để kiểm thử, test case có thể được thiết kế tùy thuộc vào tình hình, hoặc hoặc luồng công việc trong các tài liệu mô tả chức năng hoặc khi một lỗi không mong muốn / không được mô tả trong tài liệu được tìm thấy trong khi hoạt động kiểm thử. các điều kiện điển hình để kiểm thử bao gồm chia cho số 0, để trống đầu vào, file rỗng và kiểu dữ liệu sai.

Các yếu tố được sử dụng để đoán lỗi:

* Kinh nghiệm từ những lần kiểm thử trước.
* Những khuyết thiếu (defect) trước.
* Xem lại những trường hợp đã kiểm thử.
* Giao diện người dùng.
* Kết quả của những lần test trước.
* Dựa vào những báo cáo về rủi ro của hệ thống hoặc của phần mềm.
* Dựa vào các loại dữ liệu được sử dụng để test.

Mặc dù, đoán lỗi là một trong những kỹ thuật chính trong kiểm thử nhưng không bao quát đầy đủ được hệ thống, cũng không thể đảm bảo hệ thống đạt được chất lượng như mong đợi. Do vậy nên kết hợp với các kỹ thuật khác để mang lại hiệu quả tốt hơn.

## 2. Kiểm thử thăm dò(Exploratory testing) <a href="#22-ki-e1-bb-83m-th-e1-bb-ad-th-c4-83m-d-c3-b2exploratory-testing" id="22-ki-e1-bb-83m-th-e1-bb-ad-th-c4-83m-d-c3-b2exploratory-testing"></a>

Đối với kiểm thử thông thường, theo kịch bản có sẵn, bạn sẽ thiết kế test case trước, sau đó tiến hành thực hiện kiểm thử. Ngược lại, kiểm thử thăm dò là việc thực hiện đồng thời thiết kế và thực hiện kiểm thử.

Kiểm thử thăm dò bao gồm tất cả các việc như: phát hiện lỗi, điều tra lỗi, sự hiểu biết về ứng dụng. Điều này chú trọng vào sự tự do cá nhân và trách nhiệm của từng nhân viên. Test cases có thể không được tạo hoàn chỉnh nhưng người thực hiện vẫn có thể kiểm tra hệ thống một cách nhanh chóng. Họ có thể ghi lại ngắn gọn những gì mình cần làm trước khi thực hiện kiểm thử. Kiểm thử thăm dò tập trung nhiều hơn vào việc thực hiện kiểm thử hơn là tạo test cases.

_**Kiểm thử thăm dò :**_

* Không phải là kiểm thử ngẫu nhiên nhưng nó là kiểm thử mang tính bột phát với mục đích tìm được các lỗi.
* Có cấu trúc và chặt chẽ.
* Dễ dàng quản lý.
* Không phải là một kĩ thuật nhưng là một phương pháp tiếp cận. Những hành động bạn thực hiện tiếp theo được điều chỉnh bởi những gì bạn đang làm.

Một khía cạnh quan trọng của kiểm thử thăm dò là học hỏi: học hỏi người kiểm thử về phần mềm, cách sử dụng, điểm mạnh và điểm yếu của hệ thống. kiểm thử thăm dò là dò xét, tìm hiểu về phần mềm, hệ thống làm những gì và không làm những gì, những bộ phận nào làm việc và bộ phận nào không làm việc. Người kiểm thử liên tục liên tục đưa ra quyết định về những vấn đề kiểm tra tiếp theo và nơi để chi tiêu thời gian.

_**Ưu điểm:**_

* Phương pháp này không yêu cầu chuẩn bị cho quá trình test như là việc chúng ta không có tài liệu cho hoạt động kiểm thử.
* Thời gian trong quá trình test được tiết kiệm do tất cả các nhiệm vụ test được làm cùng một lúc như là quá trình test, thiết kế kịch bản kiểm thử và thực hiện các kịch bản kiểm thử.
* Nhân viên kiểm thử (QA) có thể báo cáo nhiều vấn đề do yêu cầu không đầy đủ hoặc tài liệu yêu cầu còn thiếu.

_**Nhược điểm:**_

* Vài vấn đề không thể được khai thác trong kiểu test này.
* Có xem xét lại các kế hoạch kiểm tra và thiết kế testcase/kịch bản test trong khi quá trình test có xảy ra vấn đề.
* Những nhân viên kiểm thử (QA) cần phải nhớ kịch bản test - những gì đang thực hiện test bởi vì nếu có lỗi được tìm thấy, tester (QA) sẽ “report a bug” với các bước thích hợp để tái hiện lại nó, với các lỗi khó tái hiện cần phải mô tả các bước một cách thích hợp để thực hiện một cách chính xác lỗi mà anh ta đã báo cáo đặc biệt là với các lỗi mới được tìm thấy.
