# Requirement Traceability Matrix

Writer: Datdt

## **Introduction** <a href="#introduction" id="introduction"></a>

### Overview:

Requirement Traceability Matrix là một tài liệu dưới dạng bảng (or spreadsheet) đồng liên quan bất kỳ hai hay nhiều tài liệu cơ bản đòi hỏi một mối quan hệ nhiều-nhiều để kiểm tra tính đầy đủ của các mối quan hệ. Nghĩa là để đảm bảo rằng tất cả mọi thứ trong phạm vi của các tài liệu có liên quan, nó được sử dụng để theo dõi các req và kiểm tra các req này đã được đáp ứng đủ hay chưa. Có thể xác định được các req nào sinh ra nhiều lỗi nhất trong quá trình kiểm thử.

### Mục đích:

* Đảm bảo độ bao phủ tuyệt đối: Tất cả requirement cần phải được bao phủ trong Test Design và trong quá trình thực hiện test. Mục đích là đảm bảo cover được 100% trường hợp kiểm thử.
* Theo dõi thay đổi yêu cầu: Duy trì trong suốt vòng đời của việc phát hành, thay đổi các yêu cầu này cũng được ghi lại và theo dõi trong RTM.
* Quản lý rủi ro: đảm bảo rằng mỗi requirement có thể được test và cuối cùng phải được test.
* Phát hiện và đề xuất chức năng bị miss.
* Tasks: Trợ giúp trong việc tạo ra các tài liệu về yêu cầu, spec, các tài liệu bàn giao, và plan dự án.
* Khả năng bảo trì: Bất kỳ sự thay đổi yêu cầu nào đều có thể theo dõi được để cập nhật trong Test Design.
* Bám theo scope: Sử dụng việc đảo ngược việc truy xuất để đảm bảo rằng không có kiểm thử thêm nào được thực hiện mà không có một yêu cầu tương ứng.
* Đánh dấu bất kỳ yêu cầu không rõ ràng (thiếu)
* Chất lượng sản phẩm: Phạm vi kiểm thử và tình trạng lỗi tương ứng tìm ra tạo thêm niềm tin cho khách hàng về chất lượng của sản phẩm.
* Ước tính yêu cầu thay đổi: Sử dụng RTM, Test Manager có thể dễ dàng đánh giá tác động và số lượng công việc cần thiết nếu có bất kỳ yêu cầu thay đổi nào.
* Chất lượng của thành phần: Cần đánh giá được các component nào có nguy cơ xảy ra nhiều lỗi nhất, một cách khác để đánh dấu các khu vực có nguy cơ cao cần được kiểm tra kỹ hơn.

### Phân loại:

*   Forward traceability (Truy xuất nguồn gốc xuôi): Được sử dụng để kiểm thử xem dự án có tiến triển theo hướng mong muốn và cho đúng sản phẩm hay không, đảm bảo rằng mỗi yêu cầu được áp dụng cho sản phẩm và từng yêu cầu được kiểm thử kỹ lưỡng. Nó ánh xạ các yêu cầu để kiểm thử các trường hợp.​​

    <figure><img src="../.gitbook/assets/image (49).png" alt=""><figcaption></figcaption></figure>
*   Backward or reverse traceability (Truy xuất nguồn gốc ngược): Được sử dụng để đảm bảo liệu sản phẩm hiện tại có đi đúng hướng hay không. Mục đích của Backward or reverse traceability là để xác minh rằng chúng ta không mở rộng phạm vi của dự án bằng cách thêm code, các thành phần thiết kế, kiểm thử hoặc công việc khác không được chỉ định trong các yêu cầu. Nó ánh xạ các test cases theo yêu cầu.​​

    <figure><img src="../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>
*   Bi-directional traceability (Truy xuất nguồn gốc hai chiều): Đảm bảo rằng tất cả các yêu cầu được bao phủ trong các test case, phân tích tác động của sự thay đổi trong các yêu cầu bị ảnh hưởng bởi lỗi trong sản phẩm và ngược lại.​​

    <figure><img src="../.gitbook/assets/image (31).png" alt=""><figcaption></figcaption></figure>

### Lợi ích:

1. Quản lý phạm vi giải pháp
2. Đánh giá nhanh các thay đổi tiềm năng
3. Giảm rủi ro dự án
4. Tăng cường sự nhất quán giữa các yêu cầu
5. Cho phép theo dõi và kiểm soát trong suốt vòng đời của các yêu cầu

...

### Đối tượng sử dụng:

Tài liệu sử dụng cho tất cả thành viên trong Symper để có thể hiểu được việc truy xuất nguồn gốc có ý nghĩa và mục đích ra sao và áp dụng vào nội bộ

### Sơ đồ vai trò

|                           |                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| What                      | Một bảng được sử dụng để theo dõi từng yêu cầu trở lại các quy trình và mục tiêu kinh doanh hỗ trợ và chuyển tiếp đến các tạo tác, sự kiện và các mục cấu hình đã thay đổi tiếp theo do kết quả của nó.                                                                                                                                                                                                                                                               |
| When                      | <p>Initiation:Senior BA determines what will be traced; sets up traceability matrix for the project.</p><p>Discovery:Updated by team members.</p><p>Construction: Khi các yêu cầu được thiết kế, mã hóa và thử nghiệm, ma trận được cập nhật để phù hợp với đặc điểm kỹ thuật thiết kế kết quả, các bảng đã thay đổi, các trường hợp thử nghiệm, v.v.</p>                                                                                                             |
| Where                     | Có thể là một tài liệu (chẳng hạn như bảng hoặc bảng tính) hoặc nằm trong bộ quản lý yêu cầu hoặc Hệ thống quản lý cấu hình                                                                                                                                                                                                                                                                                                                                           |
| Why                       | <p>• Cung cấp khả năng đảm bảo không có yêu cầu nào trượt qua các vết nứt bằng cách truy tìm các yêu cầu chuyển tiếp đến các trường hợp kiểm thử, đơn vị phần mềm đã thay đổi, v.v.</p><p>• Cung cấp khả năng phân tích tác động thượng nguồn và hạ nguồn của các thay đổi. Ví dụ: lặp lại tác động kinh doanh của một thay đổi CNTT (chẳng hạn như việc hủy bỏ một dự án CNTT) để phản hồi ngược trở lại quy trình kinh doanh, mục tiêu, mục tiêu và khách hàng.</p> |
| What to show stakeholders | Được sử dụng làm đầu vào cho các báo cáo trạng thái.                                                                                                                                                                                                                                                                                                                                                                                                                  |
| What to show team members | Làm cho bảng có thể truy cập để các thành viên trong nhóm xem.                                                                                                                                                                                                                                                                                                                                                                                                        |
| Complementary tools       | Requirements attributes table​                                                                                                                                                                                                                                                                                                                                                                                                                                        |

References:

https://www.perforce.com/resources/alm/requirements-traceability-matrix

#### **Định nghĩa:**

* **RTM: Requirement Traceability Matrix**
* **SRS: System Requirement Specification**
* **ERD: Entity Relationship Diagram**

**Một ví dụ đơn giản cho RTM dành cho Test case để truy ngược về Requirement để kiểm tra xem đã được test chưa và tình trạng requirement xuyên suốt dự án đó ra sao bằng cách map 2 Test case và Req lại với nhau**

<figure><img src="../.gitbook/assets/image (36).png" alt=""><figcaption></figcaption></figure>

**hoặc trình bày ở dạng báo cáo:**

<figure><img src="../.gitbook/assets/image (35).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../.gitbook/assets/image (13) (1).png" alt=""><figcaption></figcaption></figure>

## **High Level Requirement**

#### **Tổng quan luồng công việc**

#### **Mối quan hệ**

**Các thực thể có trong database, và mối quan hệ giữa chúng với nhau.**

***

**Mô hình ERD**\\

***

#### **Workflow Diagram**

**Luồng công việc và các bước được thực hiện bởi mỗi User trong Hệ Thống**

* **B1: Thu thập, xử lý tài liệu BRD, SRS, FRD, User Story,...**
* **B2: Liệt kê, phân loại tất cả các req trong 1 doc**
* **B3: Thêm một cột để biết req đó được xác thực hay không, được theo dõi và xác nhận thì đánh dấu**
* **B4: Thêm tất cả những req đã được xác định vào doc req của hệ thống**
* **B5: Chốt req và thêm những req đã được xác định ở bước trước vào trong sprint tháng**
* **B6: Viết Test Scenario và Test Case**
* **B8: Tổng hợp vào bảng Requirement Traceability Matrix**
* **B9: Kiểm tra các lỗ hổng trên ma trận, requirement, kịch bản kiểm thử hoặc test case không liên quan đến phần nào cần phải truy xuất và xử lý**
* **B10: Cập nhật RTM, ID,....**

**Triển khai thực tế trong Symper**

* **B1: BA nhận, tổng hợp các tài liệu high level req từ Stakeholders, thêm một cột để đánh giá tính khả dụng, xác nhận req**

**VD**

| Business requirement | Module name                      | User role                                                   | Description                                                                                                                                                                                                                                                                                                                             |
| -------------------- | -------------------------------- | ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **BR1**              | **Application Login and Logout** | <p><strong>Student, Professor, Dean, Staff</strong><br></p> | <p><strong>Một sinh viên có thể đăng nhập bằng tên người dùng và mật khẩu chính xác chỉ khi vai trò người dùng được chọn là 'Sinh viên'. Tương tự, áp dụng cho vai trò người dùng là Giáo sư, Trưởng khoa và Nhân viên.</strong><br></p>                                                                                                |
| BR2                  | Profile page                     | <p><strong>Student, Professor, Dean, Staff</strong><br></p> | <p><strong>Sinh viên, Giáo sư, Trưởng khoa và Nhân viên khi đăng nhập thành công có thể thấy chi tiết hồ sơ của họ chứ không phải các hồ sơ khác.</strong><br></p>                                                                                                                                                                      |
| BR3                  | Task Assignment                  | **Student, Professor, Dean, Staff**                         | <p><strong>Sinh viên có thể chấp nhận hoặc từ chối các bài tập do Giáo sư giao. Trưởng khoa có thể chấp thuận và không chấp thuận nhiệm vụ được giao bởi giáo sư. Giáo sư có thể phê duyệt và từ chối bài tập do Sinh viên nộp. Nhân viên phải nắm bắt điểm và điểm do giáo sư đệ trình đối với bài tập của sinh viên.</strong><br></p> |

***

* **B2: BA chia nhỏ, liệt kê Req cho từng project vào doc req của Symper**

**(Req. ID & Description)**

<figure><img src="../.gitbook/assets/image (25).png" alt=""><figcaption></figcaption></figure>

**Ví dụ:**

| Req ID  | Description                                                                                                    |
| ------- | -------------------------------------------------------------------------------------------------------------- |
| **SR1** | **ID người dùng là trường bắt buộc và không được để trống.**                                                   |
| SR2     | **Mật khẩu là trường bắt buộc và không được để trống.**                                                        |
| SR3     | **Vai trò người dùng là một trường bắt buộc và nên được chọn trong số Student, Professor, Dean, Staff**        |
| SR4     | **ID người dùng, mật khẩu và vai trò người dùng hợp lệ. Đăng nhập thành công.**                                |
| SR5     | **Nếu ID Người dùng hoặc Mật khẩu sai nhưng Vai trò Người dùng vẫn hợp lệ. Đăng nhập không thành công.**       |
| SR6     | **Nếu ID người dùng và Mật khẩu chính xác nhưng Vai trò người dùng không hợp lệ. Đăng nhập không thành công.** |
| **SR7** | **Student, Professor, Dean, Staff có thể xem trang hồ sơ tiếp nhận của họ.**                                   |
| SR8     | **Nhiệm vụ Phân công chỉ có thể được giao bởi Professor**                                                      |
| SR9     | **Học sinh có thể chấp nhận hoặc từ chối Nhiệm vụ được giao.**                                                 |
| SR10    | **Trưởng khoa có thể chấp thuận hoặc không chấp nhận nhiệm vụ được Sinh viên chấp nhận.**                      |
| SR11    | **Giáo sư có thể chấp thuận hoặc không chấp thuận bài tập do Sinh viên nộp.**                                  |
| SR12    | **Nhân viên có thể nắm bắt điểm hoặc điểm do Giáo sư cung cấp đối với bài tập của Học sinh.**                  |

**B3: Team BA và team DEV sẽ chốt req để đưa vào sprint phân công cho từng DEV và BA phụ trách từng đầu req**

<figure><img src="../.gitbook/assets/image (21) (1).png" alt=""><figcaption></figcaption></figure>

**B4: Track những req đã hoàn thành trong sprint để team QA, QC tạo kịch bản kiểm thử (Test Scenario)**

**VD:**

**TS1: Kiểm tra chức năng đăng nhập**

| Req ID  | TS ID | TC ID | TC name                                                                   |
| ------- | ----- | ----- | ------------------------------------------------------------------------- |
| **SR4** | TS1   | TC1   | Đăng nhập thành                                                           |
| SR5     | TS1   | TC2   | **Đăng nhập không thành công do tên người dùng và mật khẩu không hợp lệ** |
| SR6     | TS1   | TC3   | **Đăng nhập không thành công do vai trò người dùng không hợp lệ**         |

**QC viết test case và thực hiện test case trên doc của hệ thống symper (doc 2230):**

* QC điền REQ ID, các sub id sẽ nhảy ra trong bảng

<figure><img src="../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

**B5: Hoàn thành bảng quan hệ cho tất cả các trường hợp nhưng chỉ lấy các cột ID (hệ thống tự xử lý)**

**=> RTM**

| BR      | SR  | Test Scenario | Test case |
| ------- | --- | ------------- | --------- |
| **BR1** | SR4 | TS1           | TC1       |
| BR1     | SR5 | TS1           | TC2       |
| BR1     | SR6 | TS1           | TC3       |

<figure><img src="../.gitbook/assets/image (52).png" alt=""><figcaption></figcaption></figure>

**=> có thể truy xuất được các dữ liệu từ bảng trên:**

**Ví dụ:**

* Trạng thái Req đều là TO-DO (Tức req chưa được hoàn thành) nhưng đều đã có Test Case => Sai về mặt logic. Truy xuất đến trạng thái là do chưa cập nhật hay là thực tế đang TO-DO mà QC đã test
* có một số Test Case không có requirement ID => Lí do k có req id là gì: QC test những chức năng không được lên req cụ thể trên hệ thống mà dựa vào kịch bản được dựng trước để có thể bao phủ toàn bộ module
* Ở ô Cycle sẽ cho biết req này đang phải xử lý Test case quá nhiều lần (2, 3, 4,...) => Cần kiểm tra req xem có vấn đề gì không,.... dựa vào báo cáo truy ra được là của BA nào lên req và của DEV nào đang code, có bị conflict nhau không?
* Số lượng bug lặp lại ở req,.... updating, bổ sung vào ver 2

**Yêu cầu vận hành**: Khi BA report bug phải báo được với QC về ID ISSUE để QC có thể điền Test Case ID
