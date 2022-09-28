---
description: Thanhntp
---

# Kiểm thử tĩnh

## 1. Static testing là gì? <a href="#_1-static-testing-la-gi-0" id="_1-static-testing-la-gi-0"></a>

* Ngược lại với dymanic testing (kiểm thử động), kiểm thử động yêu cầu phải chạy phần mềm để test. Còn kiểm thử tĩnh là kĩ thuật kiểm tra các tài liệu (review) và tự động phân tích cú pháp (static analysis) của code hoặc các tài liệu của dự án mà không cần chạy chương trình.
* Cả 2 kĩ thuật của kiểm thử tĩnh đều thực hiện đánh giá code và các work product khác mà không cần thực hiện chạy code.
* Static analysis là quan trọng cho hệ thống đòi hỏi tiêu chí an toàn cao, ví dụ như các phần mềm về hàng không, y khoa...
* Những work product có thể được kiểm tra bởi kiểm thử tĩnh:
  * Đặc tả yêu cầu: requirements, functional requirements, security requirements
  * User stories, acceptance criteria (tiêu chí chấp nhận)
  * Code
  * Tài liệu thiết kế và kiến trúc...
* Review áp dụng cho bất kì work product mà người tham gia cần phải đọc và hiểu.
* Static analysis có thể được áp dụng hiệu quả cho bất kì work product nào có cấu trúc tiêu chuẩn (thông thường như code hoặc models), với mỗi work product mà có công cụ phân tích tĩnh phù hợp. Static analysis thậm chí có thể áp dụng với những tool đánh giá work product với ngôn ngữ tự nhiên giống như requirement (ví dụ như kiểm tra chính tả, cú pháp...).

### 1.1 Lợi ích của static testing

* Kĩ thuật kiểm thử tĩnh cung cấp rất nhiều lợi ích. Khi áp dụng sớm vào vòng đời phát triển phần mềm, kiểm thử tĩnh có khả năng xác định sớm những defect trước khi thực hiện kiểm thử động (ví dụ các defect trong quá trình review tài liệu requirement, design...)
* Các defect được phát hiện sớm thì chi phí để remove sẽ rẻ hơn nhiều so với việc tìm thấy muộn trong vòng đời phát triển phần mềm, đặc biệt khi so với chi phí bỏ ra khi các defect được phát hiện sau khi phần mềm được deployed và được đưa vào sử dụng.
* Cụ thể các lợi ích của static testing bao gồm:
  * Phát hiện và sửa lỗi hiệu quả hơn trước khi thực hiện kiểm thử động
  * Ngăn chặn những defect trong thiết kế và code bằng cách phát hiện ra sự mâu thuẫn, mơ hồ, thiếu sót, không chính xác.
  * Xác định những defect mà không dễ dàng phát hiện bởi kiểm thử động
  * Tăng hiệu suất phát triển: ví dụ do thiết kế được cải tiến, code dễ bảo trì
  * Giảm thời gian và chi phí phát triển
  * Giảm thời gian và chi phí test

### 1.2 Sự khác nhau giữa kiểm thử tĩnh và kiểm thử động

* Static testing và dymanic testing có cùng mục đích, như là cung cấp đánh giá về chất lượng của work product và xác định defect càng sớm càng tốt.
* Hai phương pháp này bổ trợ cho nhau vì tìm thấy các defect khác nhau.
* Điểm phân biệt chính là kiểm thử tĩnh tìm kiếm defect trong work product 1 cách trực tiếp còn kiểm thử động xác định các failures gây ra bởi defect khi chạy phần mềm.
* Một defect có thể tồn tại trong work product 1 thời gian dài mà không gây ra failure
* Kiểm thử tĩnh có thể tìm thấy defect mà tốn ít công sức hơn
* Một điểm khác nhau nữa là kiểm thử tĩnh có thể được sử dụng để nâng cao tính nhất quán và chất lượng bên trong của work product, trong khi kiểm thử động thông thường tập trung vào hành vi bên ngoài của sản phẩm.
* Khi so sánh với kiểm thử động, các loại defect đặc thù mà có thể tìm thấy và fix 1 cách dễ dàng và chi phí rẻ bao gồm:
  * Requirement defects (ví dụ: mâu thuẫn, dư thừa, không chính xác)
  * Design defects (thuật toán hoặc cấu trúc dữ liệu không hiệu quả)
  * Coding defects (các biến có giá trị không xác định, các biến được khai báo nhưng không sử dụng, code không thể truy cập, code trùng lặp)
  * Độ lệch so với tiêu chuẩn (ví dụ: thiếu tuân thủ các tiêu chuẩn code)
  * Thông số kĩ thuật giao diện không chính xác
  * Các lỗ hổng bảo mật (ví dụ: dễ tràn bộ nhớ đệm)
  * Các lỗ hổng hoặc không chính xác trong truy xuất nguồn gốc hoặc phạm vi bảo hiểm
* Ngoài ra, hầu hết các loại maintainability defects chỉ có thể tìm thấy bởi kiểm thử tĩnh.

## 2. Quá trình review

* Review có thể theo tiêu chuẩn (formal review) hoặc không theo tiêu chuẩn (informal review). Informal reviews đặc trưng bởi không tuân theo một quy trình chuẩn và không có tài liệu đầu ra tiêu chuẩn.
* Formal reviews đặc trưng thành phần tham gia, kết quả ghi chép lại của buổi review và các tài liệu ghi lại để đánh giá.
* Hình thức của quá trình review liên quan đến nhân tố như quy trình phát triển phần mềm, độ phức tạp của work product được review...
* Trọng tâm của review phụ thuộc vào các mục tiêu được thống nhất của việc review (ví dụ như tìm bug, tạo sự hiểu biết chung, đưa ra kiến thức cho người tham gia như tester/new member...

### 2.1 Quy trình review work product

#### 2.1.1 Planning (Lên kế hoạch):

* Xác định phạm vi, bao gồm mục đích của review, tài liệu hoặc một phần tài liệu nào được thực hiện review, và đặc điểm chất lượng nào cần được đánh giá.
* ước lượng nguồn lực và thời gian
* Xác định đặc điểm review như loại review tương ứng với vai trò, hoạt động và checklist
* Lựa chọn những người tham gia vào quá trình review và phân bổ vai trò
* Xác định tiêu chí đầu vào đầu ra cho mỗi loại review khác nhau
* Kiểm tra các tiêu chí đầu vào cần thiết (cho những loại review tiêu chuẩn)

#### 2.1.2 Initiate review (Khởi tạo review):

* Phân bổ work product và các phương tiện cần thiết như biểu mẫu log issue, các checklist và các tài liệu liên quan đến work product cần được review
* Giải thích giới hạn, mục đích, quy trình, vai trò và các work product cho người tham gia review
* Giải đáp bất kì câu hỏi nào mà người tham gia review đưa ra về việc review

#### 2.1.3 Individual review

* Thực hiện review tất cả các phần của work product
* Ghi chú lại những defect tiềm ẩn, những đề xuất và các câu hỏi liên quan đến work product trong quá trình review

#### 2.1.4 Issue communication và analysis

* Truyền đạt những defect tiềm ẩn đã được xác định
* Phân tích các defect tiềm ẩn và giao quyền sở hữu và trạng thái cho chúng
* Đánh giá và ghi chép lại những đặc tính chất lượng
* Đánh giá những gì buổi review đem lại so với tiêu chuẩn đầu ra để tạo quyết định cho buổi review (ví dụ: reject, có sự thay đổi lớn cần phải làm, có thể chấp nhận với sự thay đổi nhỏ)

#### 2.1.5 Fixing và reporting:

* Tạo báo cáo defect cho những yêu cầu cần thay đổi
* Fix những defect được tìm thấy trong sản phẩm review
* Ghi nhận lại việc thay đổi trạng thái của defect (chỉ có trong formal review), có thể bao gồm cả sự đồng ý của người tạo comment
* Thu thập số liệu (chỉ có trong formal review)
* Kiểm tra tiêu chí đầu ra đạt được hay chưa (chỉ có trong formal review)
* Chấp nhận những work product khi tiêu chí đầu ra đã đạt được

### 2.2 Vai trò và trách nhiệm trong review tiêu chuẩn

#### 2.2.1 Author:

* Tạo ra các sản phẩm để review
* Fix các defect của work product phát hiện được trong quá trình review (nếu cần thiết)

#### 2.2.2 Manager:

* Có trách nhiệm lên kế hoạch review
* Quyết định việc thực hiện review
* Phân công người tham dự, chi phí và thời gian cho việc review
* Giám sát những chi phí phát sinh
* Thực hiện các quyết định trong trường hợp đầu ra không thỏa đáng

#### 2.2.3 Facilitator (hay còn gọi là moderator)

* Đảm bảo hiệu quả của buổi review (khi được tổ chức)
* Là người trung gian, nếu cần thiết giữa các bên khi họ có các viewpoint khác nhau
* Thường là người quyết định sự thành công của một buổi review

#### 2.2.4 Review leader

* Đảm nhận vai trò tổng thể của cuộc review
* Quyết định những ai sẽ tham gia vào buổi review và đưa ra quyết định địa điểm, thời gian cho buổi review này

#### 2.2.5 Reviewer

* Có thể là chuyên gia về một vấn đề nào đó trong work product cần review, hoặc những người trong cùng dự án, những bên liên quan quan tâm đến work product cần review hoặc những cá nhân có nền tảng kĩ thuật hoặc nghiệp vụ cụ thể liên quan đến work product cần review
* Xác định những defect tiềm ẩn trong work product thông qua việc review

#### 2.2.6 Scribe ( hoặc recorder)

* Đối chiếu/tham chiếu lại các lỗi tiềm ẩn được tìm ra trong hoạt động review cá nhân
* Ghi chép lại các lỗi tiềm ẩn mới, các điểm mở, các quyết định trong buổi họp review

### 2.3 Các loại review

#### 2.3.1 Informal review (review không theo tiêu chuẩn):

* Mục đích chính: phát hiện các defect tiềm ẩn
* Mục đích bổ sung: Tạo ý tưởng mới hoặc giải pháp mới, nhanh chóng giải quyết các vấn đề nhỏ
* Không dựa trên các quy trình tiêu chuẩn
* Có thể không bao gồm buổi họp review
* Có thể được thực hiện bởi đồng nghiệp/đồng sự của tác giả hoặc bởi nhiều người
* Kết quả review có thể ghi chép lại hoặc không
* Giá trị của buổi review phụ thuộc chủ yếu vào người review
* Có thể sử dụng checklist hoặc không
* Hay được sử dụng trong mô hình phát triển Agile

#### 2.3.2 Walkthrough

* Mục đích chính: tìm defect, cải thiện sản phẩm phần mềm, xem xét triển khai thay thế, đánh giá sự phù hợp với tiêu chuẩn và thông số kĩ thuật
* Trao đổi ý tưởng về kĩ thuật hoặc các phần cần thay đổi, đào tạo cho người tham gia, đạt cùng sự đồng thuận
* Người chủ trì cuộc họp review là tác giả của work product được review
* Vai trò Scribe là bắt buộc
* Việc log và report lại các defect tiềm ẩn có thể có hoặc không

#### 2.3.3 Technical review

* Mục đích: đạt được sự đồng thuận, xác định rủi ro tiềm ẩn
* Mục đích có thể đạt được: đánh giá chất lượng và tạo niềm tin vào sản phẩm, tạo những ý tưởng mới, thúc đẩy và cho phép tác giả cải tiến những tính năng sản phẩm trong tương lai, xem xét cần thay thế với hiện tại hay không
* Yêu cầu bắt buộc những người review cần chuẩn bị trước buổi họp review
* Buổi họp review có thể không bắt buộc, lý tưởng nhất được tổ chức với 1 moderator
* Scribe là bắt buộc
* Cần log lại những defect được phát hiện và có báo cáo review

#### 2.3.4 Inspection

* Mục đích chính: xác định defect tiềm ẩn, đánh giá chất lượng và tạo niềm tin vào sản phẩm, ngăn chặn những defect tương tự trong tương lai thông qua giúp tác giả phân tích được nguyên nhân gốc rễ.
* Mục đích có thể đạt được: thúc đẩy và cho phép tác giả cải tiến những tính năng sản phẩm trong tương lai và quy trình phát triển, đạt được sự đồng thuận
* Tuân theo một quy trình được định nghĩa sẵn với tài liệu đầu ra tiêu chuẩn, dựa trên quy tắc và checklist
* Người review hoặc đồng sự với tác giả hoặc là expert về mảng liên quan đến sản phẩm được review
* Các tiêu chí đầu vào đầu ra cần được sử dụng
* Scribe là bắt buộc
* Cần xây dựng báo cáo bug và report thông qua buổi review

### 2.4 Áp dụng các kĩ thuật vào review

#### 2.4.1 Adhoc:

* Trong kĩ thuật review Adhoc, những người review được cung cấp rất ít hoặc không có bất kì hướng dẫn nào về việc sẽ phải thực hiện task đó
* Người review thường xuyên phải đọc tài liệu một cách liên tục, xác định và ghi lại những vấn đề họ gặp phải/phát hiện được trong sản phẩm
* Adhoc là kĩ thuật thông thường nhất được sử dụng khi có rất ít sự chuẩn bị
* Kĩ thuật này phụ thuộc lớn vào kĩ năng người review và có thể gặp vấn đề rằng có 1 lượng lớn các issue bị report trùng lặp bởi các người review khác nhau.

#### 2.4.2 Checklist-based:

* Kĩ thuật review checklist-based là một kĩ thuật review có phương pháp, tức là những người review sẽ xác định issue dựa trên checklist đã được phân bổ trong giai đoạn review initiation
* Một checklist review bao gồm một tập các câu hỏi dựa trên defect tiềm tàng, thường xuất phát từ kinh nghiệm trước đó.
* Checklist sẽ được cụ thể với từng loại work product được review và thường xuyên được maintain để cover các issue bị miss tại version trước.
* Lợi ích chính của kĩ thuật checklist-based là khả năng coverage các loại defect điển hình 1 cách có hệ thống

#### 2.4.3 Scenarios và dry runs:

* Trong scenario-based review, người review được cung cấp bản hướng dẫn làm cách nào để đọc hiểu work product
* Hướng tiếp cận của scenario-based là hướng dẫn người review thực hiện "dry runs" work product dựa trên mong muốn sử dụng work product (nếu work product là tài liệu có format phù hợp ví dụ như use case)
* Phương pháp này cung cấp cho người review hướng dẫn tốt hơn về làm cách nào xác định các loại defect dễ dàng hơn so với phương pháp check list

#### 2.4.4 Role-based:

* Kĩ thuật này là người review đánh giá work product trên các quan điểm cá nhân của các bên liên quan trong dự án
* Cụ thể các vai trò này có thể là end-user (có kinh nghiệm, không có kinh nghiệm) hoặc đóng các vai trò trong tổ chức như: user administrator, system administrator, performance tester

#### 2.4.5 Perspective-based:

* Cũng tương tự như role-based, kĩ thuật này người review đứng trên góc nhìn của các bên liên quan khác nhau trong quá trình review. Các bên liên quan điển hình bao gồm: end user, marketing, designer, tester hoặc operation.. Việc sử dụng góc nhìn của các bên liên quan khác nhau có lợi ích là cái nhìn sâu hơn trong quá trình review cá nhân và cũng có tác dụng giảm bớt các issue trùng lặp
* Dựa vào các nghiên cứu đánh giá, kĩ thuật Perspective-based là có hiệu quả nhất trong việc review các tài liệu work product của hệ thống bao gồm cả yêu cầu và kĩ thuật

### 2.5 Các nhân tố thành công cho review

#### 2.5.1 Nhân tố thành công về mặt tổ chức bao gồm:

* Mỗi cuộc review phải được định nghĩa rõ ràng, đưa ra kế hoạch review, những người tham gia review và tiêu chí đo lường đầu ra để kết thúc quá trình review
* Các loại review được áp dụng cần phù hợp để đạt được mục tiêu và phù hợp với sản phẩm phần mềm và những người tham gia review
* Người tham dự cần có thời gian đầy đủ để chuẩn bị
* Việc review được lập lịch với thông báo đầy đủ tới những người tham gia

#### 2.5.2 Nhân tố về con người liên quan đến việc review:

* Mời đúng những người cần tham gia review để đạt được mục đích review cụ thể ví dụ như mời những người có kĩ năng hoặc có góc nhìn khác nhau
* Tester là người rất có giá trị khi tham gia vào review và cũng để học luôn về work product, cái mà cần chuẩn bị tốt cho việc test hiệu quả và chuẩn bị cho việc test sớm
* Buổi họp review cần được quản lý tốt để cho người tham dự thấy được giá trị của thời gian họ bỏ ra
