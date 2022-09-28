# Văn bản ban hành sử dụng Internal Network

## I. Phân loại

Sau khi xây dựng các quy trình, báo cáo phục vụ cho việc quản lý nội bộ (Internal network), 1 số quy trình/chứng từ/báo cáo thuộc cùng 1 nhóm đối tượng liên quan được gom vào các ứng dụng khác nhau, bao gồm:

**I.1. Project:** dùng để quản lý các công việc liên quan đến quản lý dự án

<figure><img src="../../.gitbook/assets/image (5) (1) (1).png" alt=""><figcaption></figcaption></figure>

**I.2. Symper Daily:** dùng để quản lý, theo dõi ngày làm việc cũng như công việc trong ngày của các thành viên trong team

<figure><img src="../../.gitbook/assets/image (14) (1) (1).png" alt=""><figcaption></figcaption></figure>

**I.3. Business Analyst:** dùng để quản lý các công việc liên quan đến nghiệp vụ của BA

<figure><img src="../../.gitbook/assets/image (41).png" alt=""><figcaption></figcaption></figure>

**I.4. Quality Control:** dùng để quản lý các công việc liên quan đến nghiệp vụ của QC

<figure><img src="../../.gitbook/assets/image (54) (1).png" alt=""><figcaption></figcaption></figure>

**I.5. Service and Platform Control:** dùng để theo dõi các phiên bản code kèm thay đổi chi tiết của các module, service và cả platform qua từng giai đoạn

<figure><img src="../../.gitbook/assets/image (33) (1).png" alt=""><figcaption><p><em>Hình 5. Các đối tượng trong ứng dụng Service and Platform Control</em></p></figcaption></figure>

### **II.1. Đối với các chứng từ**

Đối tượng chứng từ trong các ứng dụng dùng để theo dõi danh sách các bản ghi của các chứng từ/danh mục liên quan. **Không truy cập vào danh sách văn bản để nhập liệu trực tiếp**.

### **II.2. Đối với các quy trình**

Tất cả các nghiệp vụ phát sinh đều **phải thực hiện bằng quy trình** được chia trong các ứng dụng khác nhau mỗi khi phát sinh nhu cầu lập mới vì các trạng thái và các trường thông tin trong chứng từ được cập nhật thông qua các bước trong quy trình. Deadline lập mới các quy trình được quy định cụ thể dưới đây:

_**II.2.1. Sprint:**_ Lập mới mỗi cuối tháng

_**II.2.2. Project Charter:**_ Lập mới mỗi khi có dự án mới

_**II.2.3. WBS:**_ Nhập mới hàng ngày trước 8h30am và cập nhật/hoàn thành trước 5h30pm hàng ngày

_**II.2.4. Lịch làm việc:**_ Lập mới/đăng kí trước 8am thứ 2 hàng tuần cho tuần đó

_**II.2.5. Xin nghỉ:**_ Lập mới mỗi khi phát sinh nhu cầu xin nghỉ

_**II.2.6. Requirement:**_ Lập mới mỗi khi phát sinh yêu cầu mới/ thay đổi yêu cầu cho hệ thống/nghiệp vụ. Các requirment chưa được tạo trên hệ thống sẽ không được merge code.

_**II.2.7. Issue Tracking:**_ Lập mới mỗi khi phát sinh vấn đề: lỗi hệ thống, lỗi thiết kế, lỗi nghiệp vụ, ghi nhận meeting notes,.... Các bug sẽ không được fix nếu chưa được tạo trên hệ thống.

_**II.2.8. Test plan:**_ Lập mới mỗi khi có test plan

_**II.2.9. Test suit:**_ Lập mới test suit dựa trên các test plan sau khi có các test plan

_**II.2.10. Test run:**_ Lập mới mỗi khi chạy 1 nhóm test cases

### **II.3. Đối với các báo cáo**

_**II.3.1. Product roadmap:**_ Mỗi khi có project mới, team leader sẽ cap màn hình và nhắn lên nhóm Symper cho team follow theo

_**II.3.2. Requirement Tracibility Matrix:**_ 2 lần 1 tháng vào thứ 2 tuần thứ 2 và 4 của tháng, Datdt cap màn hình và update tiến độ xử lý Req của team dev trong nhóm Symper

_**II.3.3. Test report:**_ QC phụ trách - Duyenntm tổng hợp báo cáo và report lên nhóm Symper theo test plan: test xong 1 plan thì họp và báo cáo với team

_**II.3.4. WBS:**_\
\- DEV & QC: Check in hàng ngày sử dụng báo cáo WBS để báo cáo, check in sáng hôm sau sẽ kiểm tra việc cập nhật các đầu việc của ngày hôm trước\
\- BA: Check in & check out hàng ngày sử dụng báo cáo WBS để báo cáo, check out 5h30pm sẽ kiểm tra kết quả công việc và cập nhật trạng thái, thời gian làm việc thực tế các đầu việc trong ngày

_**II.3.5. Issue tracking:**_ QC phụ trách - Thanhntp báo cáo các bug phát sinh theo ngày vào nhóm Symper lúc 17h30. Các bug phát sinh sau 17h30 thì để hôm sau report

_**II.3.6. Point tracking:**_ Người phụ trách - Huongntm Cuối tháng tổng kết theo sprint review

_**II.3.7. Lịch làm việc + xin nghỉ:**_ Người phụ trách - Hoanp report lịch làm việc và xin nghỉ của cả team vào 9h sáng thứ 2 hàng tuần trên nhóm Symper

_**II.3.8. Sprint:**_ COO - Tannq cập nhật bản Sprint đã chốt vào ngày đầu tiên của hàng tháng và review vào ngày cuối cùng của hàng tháng

_**II.3.9. Service version control:**_ Dev lead - Khadm tự động sinh ra bản ghi ghi nhận version mới của các service mỗi khi merge code

_**II.3.10. Platform version control:**_ Dev lead - Khadm tự động sinh ra bản ghi ghi nhận version mới của platform kèm chi tiết các thay đổi mỗi khi platform có version mới
