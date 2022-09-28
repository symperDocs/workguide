# Cơ bản về kiểm thử

## 1. Kiểm thử phần mềm là gì?

Kiểm thử phần mềm (software testing) là hoạt động nhằm tìm kiếm và phát hiện ra các lỗi của phần mềm, đảm bảo phần mềm chính xác, đúng và đầy đủ theo yêu cầu của khách hàng, yêu cầu của sản phẩm đã đặt ra. Software testing cũng cung cấp mục tiêu, cái nhìn độc lập về phần mềm điều này cho phép đánh giá và hiểu rõ các rủi ro khi thực thi phần mềm.

Kiểm thử phần mềm là phương pháp kiểm tra xem sản phẩm phần mềm đó trên thực tế có phù hợp với các yêu cầu đã đặt ra hay không và đảm bảo rằng không có lỗi hay khiếm khuyết. Nó bao gồm việc kiểm tra, phân tích, quan sát và đánh giá các khía cạnh khác nhau của sản phẩm. Người kiểm thử phần mềm (Tester) sử dụng kết hợp các công cụ thủ công và tự động. Sau khi tiến hành kiểm thử, Tester báo cáo kết quả cho team phát triển. Mục đích là xác định các lỗi, khiếm khuyết hoặc các yêu cầu còn thiếu so với yêu cầu thực tế.

### 1.1 Mục đích của kiểm thử

Đối với bất kỳ dự án nào, các mục đích của kiểm thử có thể bao gồm:

* Để ngăn ngừa các lỗi bằng cách đánh giá sản phẩm thông qua requirement, user stories, design and code
* Để xác minh rằng tất cả các yêu cầu của khách hàng được đáp ứng tốt
* Gúp nhanh chóng phát hiện các lỗi của phần mềm, giúp giảm chi phí sửa chữa
* Làm tăng độ tin cậy cho sản phẩm. Giúp hoàn thiện sản phẩm, tránh những lỗ hổng bảo mật đáng tiếc, tăng độ tin cậy cho người sử dụng

Các mục tiêu của kiểm thử có thể khác nhau, tùy thuộc vào bối cảnh của thành phần hoặc hệ thống đang thử nghiệm, mức độ thử nghiệm và mô hình vòng đời phát triển phần mềm.

### 1.2 Kiểm thử và debug

Kiểm thử và debug là khác nhau.

* Việc thực hiện kiểm thử: có thể cho thấy các lỗi gây ra bởi các lỗi trong phần mềm
* Debug: là hoạt động nhằm tìm kiếm, phân tích và sửa chữa những lỗi đó

Trong một số trường hợp, Tester chịu trách nhiệm về thử nghiệm ban đầu và kiểm tra xác nhận cuối cùng, trong khi đó Dev thực hiện gỡ lỗi, kiểm tra tích hợp thành phần và thành phần liên quan.

Tuy nhiên, trong mô hình Agile và trong một số vòng đời phát triển phần mềm khác, Tester có thể tham gia vào việc gỡ lỗi và kiểm tra thành phần.

## 2. Tại sao kiểm thử phần mềm là cần thiết?

### 2.1 **Testing’s Contributions to Success**

* Có tester tham gia vào review requirements, user story giúp phát hiện defects trong work product. Nhận diện và loại bỏ các defects trong requirements làm giảm nguy cơ của các features sai hoặc khó test đang được phát triển.
* Có tester làm việc gần với người thiết kế hệ thống khi hệ thống đang được thiết kế có thể tăng sự hiểu biết của các bên về cách thiết kế cũng như cách test chúng. Điều này sẽ giúp giảm nguy cơ về các lỗi thiết kế nền tảng và giúp xác định được lỗi từ sớm.
* Có tester làm việc gần với developers trong khi đang code có thể tăng sự hiểu biết về code cũng như cách test chúng.
* Có tester verify and validate để release có thể phát hiện ra các defects có thể bị bở sót, và hỗ trợ quy trình loại bỏ defects gây ra failure. Điều này làm tăng khả năng phần mềm đúng với thứ stakeholder cần và đúng với requirements

### **2.2 Quality Assurance and Testing**

Nhiều người thường sử dụng cụm từ Quality Assurance(QA) khi đề cập đến testing, tuy nhiên quality assurance và testing thì không giống nhưng có liên quan với nhau. Trong 1 concept rộng hơn là quản lý chất lượng, chúng luôn đi cùng với nhau:

* Quality Assurance(QA) thông thường sẽ tập trung vào sự ăn khớp của các quy trình để có thể tự tin rằng chất lượng của sản phẩm đã đạt được một mức nào đó. Trong một quy trình thích hợp, work products được tạo ra bằng quy trình đó thông th ường sẽ có chất lượng cao hơn, đóng góp vào bug prevention. Thêm vào đó, việc sử dụng Root cause analysis và các buổi retrospective meetings là quan trọng để cải thiện quy trình.
* Quality Control(QC) bao gồm nhiều hoạt động, bao gồm các hoạt động test, giúp đạt được các mức độ về chất lượng . Các hoạt động test là một phần của quy trình phát triển và bảo trì phần mềm. Testing đóng góp vào việc thành công của chất lượng phần mềm.

### 2.3 **Phân biệt Errors, Defect và Failures**

* Error: là lỗi lầm xuất phát từ con người trong việc đọc, hiểu, truyền đạt các yêu cầu (requiement).
* Defect **** (fault/bug): là việc những phần code sai được tạo ra bởi những error trên
* Failure: là những lỗi nằm trên phần mềm đang được chạy

**Các lí do gây ra error:**

* Áp lực về thời gian
* Lỗi của con người
* Không/thiếu kinh nghiệm của các thành viên tham gia project
* Sự truyền đạt thông tin sai lệch giữa các thành viên về yêu cầu và thiết kế
* Sự phức tạp của code, thiết kế, kiến trúc hệ thống và các công nghệ/ nền tảng
* Lỗi kết nối/giao tiếp của các hệ thống có nhiều hệ thống con
* Sử dụng các công nghệ mới/ không quen thuộc

Ngoài những failures gây ra bởi defect, thì các điều kiện môi trường cũng có thê gây ra lỗi.

**Phân biệt false positives và false negative:**

* False positives: là các phát hiện không phải là failure nhưng được report là failure. Có thể là do test sai cách, sai test data, sai môi trường test…
* False negatives: là các failure tồn tại trong hệ thống, nên được tìm ra nhưng lại bị bỏ sót trong quá trình test

### **2.4 Defect, Root Causes and Effects**

Root Cause là hành động sai sớm nhất gây ra defects. Các defects cần được phân tích để xác định root cause để mà giảm các defect tương tự trong tương lai. Bằng việc tập trung vào các root cause nổi bật, root cause analysis có thể giúp cải tiến quy trình nhằm giảm các defects có thể xảy ra sau này.&#x20;

Effect: là các hậu quả của việc phần mềm có lỗi khi đã đưa vào vận hành.

Ví dụ: Khách hàng phàn nàn về việc phần lãi suất bị tính sai bởi vì một dòng code sai. Dòng code này bị sai này thuộc một user story nhập nhằng vì Product Owner(PO) hiểu sai cách tính lãi suất. Nếu như có một số lượng lớn defects xảy ra vì lí do này, PO nên được đào tạo lại về cách tính lãi suất nhằm giảm thiểu các sai sót tương tư trong tương lai. Trong ví dụ này:

* Effects: là việc bị khách hàng phàn nàn
* Failure: là hệ thống tính ra sai lãi suất
* Defects: là dòng code tính toán sai kia
* Errors: là lỗi lầm của PO tạo ra user story sai
* Root cause: việc thiểu hiểu biết của PO về tính lãi suất
* Root cause analysis: là việc xác định root cause xảy ra đầu tiên có nguồn gốc từ đâu
* Improvement: PO được đào tạo thêm về nghiệp vụ; dev được khuyến khích hỏi lại PO, PM nếu cảm thấy requiements mơ hồ, nhập nhằng…

## 3. 7 nguyên tắc kiểm thử là gì?

### 3.1 Kiểm thử để đưa ra lỗi của phần mềm

Mục đích của kiểm thử là chứng minh lỗi của phần mềm, không phải chứng minh phần mềm đã hết lỗi. Vì thế, việc thiết kế một chiến lược kiểm thử với độ bao phủ tốt sẽ giúp giảm thiểu các lỗi khi đưa sản phẩm ra thị trường.

### 3.2 Kiểm thử toàn bộ là không thể

Kiểm thử toàn bộ hệ thống là một yêu cầu bất khả thi. Thay vào đó, Tester sẽ tập trung vào các chức năng, các phân hệ dễ xảy ra lỗi của hệ thống. Việc dự đoán các rủi ro là một trong những kỹ năng cần thiết của Tester và được học hỏi, tích lũy trong quá trình làm việc.

### 3.3 Kiểm thử càng sớm càng tốt

Trong quy trình phát triển phần mềm, triển khai kiểm thử ở giai đoạn đầu sẽ giúp giảm thiểu rủi ro, các bug được phát hiện sớm, tránh tình trạng tích hợp vào gây lỗi trên nhiều module.

### 3.4 Lỗi thường phân bổ tập trung

"80% số lượng lỗi được tìm thấy trong 20% tính năng của hệ thống". Thông thường, các lỗi sẽ tập trung ở một số module, chức năng chính của hệ thống. Do đó, khi phát hiện lỗi, Tester nên tập trung kiểm tra các chức năng có liên quan để có thể phát hiện các lỗi mới. Đây cũng là một trong những phương pháp tăng hiệu quả của giai đoạn kiểm thử.

### 3.5 Nguyên tắc "Thuốc trừ sâu"

Việc sử dụng nhiều lần làm các trường hợp kiểm thử sẽ làm giảm khả năng phát hiện lỗi. Bởi phát triển phần mềm là một quy trình được kế thừa qua nhiều giai đoạn, các lỗi được phát hiện nhờ các trường hợp trên có thể đã được sửa. Do đó, cần phải thường xuyên cập nhật, thay đổi test case để đảm bảo đáp ứng sự thay đổi của hệ thống.

### 3.6 Kiểm thử phụ thuộc vào ngữ cảnh

Việc đưa ra chiến lược kiểm thử phù hợp phụ thuộc vào từng hoàn cảnh khác nhau. Việc kiểm thử ứng dụng Web, Mobile hay Web service sẽ có các kỹ thuật tương ứng. Cùng với đó, trong từng lĩnh vực (tài chính, y tế, giáo dục ...) cũng có những cách tiếp cận phù hợp.

### 3.7 Phần mềm không có lỗi là quan niệm sai lầm

Mục đích của kiểm thử là chứng minh lỗi của phần mềm, không phải chứng minh phần mềm đã hết lỗi. Vì kiểm thử toàn bộ là không thể, do đó phần mềm có thể sẽ còn các lỗi tiềm ẩn hoặc chưa được phát triển.

## 4. Quy trình test

Chúng ta không có một quy trình test phần mềm phổ thông nào, nhưng sẽ có một danh sách các hoạt động phổ biến không thể thiếu được trong quá trình test nếu muốn đạt được một số mục tiêu đã thiết lập.

### 4.1 Ngữ cảnh Test Process

Các yếu tố ngữ cảnh ảnh hưởng đến quy trình test cho một tổ chức bao gồm:

* Loại mô hình phát triển phần mềm và phương pháp thực hiện mà dự án sử dụng
* Test levels và test types được xem xét
* Các rủi ro về sản phẩm và dự án
* Business domain
* Những hạn chế của việc vận hành (Kinh phí và nguồn lực, Thời gian, Độ phức tạp, Các yêu cầu về hợp đồng và quy định)

### 4.2 Hoạt động và nhiệm vụ của kiểm thử

Một chu trình test bao gồm nhóm các hoạt động chính sau:&#x20;

* Test planning
* Test monitoring and control
* Test analysis
* Test design
* Test implementation
* Test execution
* Test completion

#### 4.2.1 Test planning

Tập trung vào việc định nghĩa mục đích của testing, cách tiếp cận để đáp ứng các mục tiêu testing trong các ràng buộc được đặt ra bởi bối cảnh.

Test plans nên được xem xét lại dự trên feedback của hoạt động monitoring và control.

#### 4.2.2 Test monitoring and control

Tập trung chủ yếu vào so sánh liên tục giữa tình hình thực tế và kế hoạch đưa ra sử dụng những metrics được định nghĩa trong test plan để giám sát.

#### 4.2.3 Test analysis

Trong quá trình test analysis, các test basic được phân tích để xác định những tính năng nào có thể test được và xác định những điều kiện test tương ứng.

Gồm những task chính:

* Phân tích các test basic phù hợp với test level đang được xem xét
* Đánh giá các test basic và test item để xác định một sốt loại defect khác nhau
* Xác định những tính năng được test
* Xác định và đưa thứ tự ưu tiên của các điều kiện cho mỗi tính năng

#### 4.2.4 Test design

Gồm những task chính sau:

* Thiết kế và đánh mức độ ưu tiên Test case
* Xác định data test cần thiết để hỗ trợ điều kiện test
* Thiết kế môi trường và xác định các tool cần thiết

#### 4.2.5 Test implementation

Gồm những task chính sau:

* Phát triển và phân loại thứ tự ưu tiên của quy trình test và tạo test script nếu cần
* Tạo test suites từ test procedures
* Sắp xếp test suites trong quá trình thực hiện test
* Tạo môi trường test và xác nhận tất cả mọi thứ cần thiết đều được cài đặt chính xác
* Chuẩn bị data test

#### 4.2.6 Test execution

Gồm những task chính sau:

* Thực hiện test thủ công hoặc sử dụng tool
* So sánh kết quả thực tế và kết quả mong muốn
* Phân tích các vấn đề bất thường để phát hiện các lỗi
* Báo cáo lỗi

#### 4.2.7 Test completion

Gồm những hoạt động sau:

* Kiểm tra đảm bảo rằng tất cả các lỗi đều được closed, thêm những yêu cầu thay đổi hoặc product backlog items cho những lỗi nào mà chưa được giải quyết khi kết thúc hoạt động test execution
* Tạo test summary report để giao tiếp với các stakeholder
* Hoàn thiện và lưu trữ môi trương test, data test
* Bàn giao testware cho nhóm bảo trì, đội dự án
* Phân tích bài học rút ra từ hoạt động để xác định những việc cần thay đổi trong dự án, bản release, chu kỳ tiếp theo
* Sử dụng thông tin thu thập được để cải thiện độ trưởng thành của process

### 4.3 Test Work Products (TWP)

TWP là một phần quan trọng trong quá trình kiểm thử, bởi vì có nhiều cách để thực hiện TWP, nên các sản phẩm công việc được tạo ra cũng khác nhau ở các bước tổ chức và thực hiện.

#### 4.3.1 Test planning work products (TPWP)

TPWP thường bao gồm một hoặc nhiều chiến lược test.

Kế hoạch kiểm thử bao gồm thông tin về cơ sở thử nghiệm, trong đó các sản phẩm công việc kiểm thử khác sẽ liên quan đến thông tin truy suất nguồn gốc cũng như các tiêu chuẩn dừng test (hay còn gọi là định nghĩa hoàn thành) được sử dụng trong quá trình kiểm thử.

#### 4.3.2 Test monitoring and control work products

Các sản phẩm của việc kiểm soát test và giám sát công việc thường bao gồm nhiều loại báo cáo thử nghiệm khác nhau, bao gồm báo cáo tiến độ thử nghiệm (được tạo ra liên tục và/hoặc thường xuyên) và báo cáo tóm tắt thử nghiệm (được tạo ra ở mốc hoàn thành khác nhau).

Tất cả các báo cáo thử nghiệm phải cung cấp chi tiết liên quan đến đối tượng đọc báo cáo về tiến trình thử nghiệm kể từ ngày báo cáo, bao gồm cả việc tóm tắt kết quả thực hiện thử nghiệm ngay khi có thể.

Các sản phẩm của việc kiểm soát test và giám sát công việc cũng nên bao gồm các vấn đề quan trọng trong quản lý dự án, chẳng hạn như việc hoàn thành task được giao, phân bổ và sử dụng tài nguyên các tài nguyên cũng như effort của các thành viên dự án.

#### 4.3.3 Test analysis work products

Test analysis work products bao gồm các điều kiện thử nghiệm được xác định rõ ràng và được đánh số ưu tiên, các điều kiện này nên được truy vấn hai chiều tùy theo đối tượng của cơ sở kiểm thử.

Đối với exploratory testing, phân tích thử nghiệm có thể liên quan đến việc tạo ra các test charter. Phân tích thử nghiệm cũng có thể dẫn đến việc phát hiện và báo cáo defect trong test basis.

#### 4.3.4 Test design work products

Kết quả của thiết kế thử nghiệm là test case và các bộ test case để thực hiện các điều kiện thử nghiệm được xác định trong phân tích thử nghiệm.

Nó thường là một thực hành tốt để thiết kế high-level test case, không có giá trị cụ thể cho dữ liệu đầu vào và kết quả mong đợi.

Các high-level test case như vậy có thể được sử dụng lại qua nhiều chu kỳ thử nghiệm với dữ liệu cụ thể khác nhau, trong khi vẫn ghi lại đầy đủ phạm vi của test case.

#### 4.3.5 Test implementation work products

Test implementation work products bao gồm:

* Quy trình thử nghiệm và giải trình tự các quy trình thử nghiệm đó
* Bộ kiểm thử
* Lịch thực hiện kiểm thử

#### 4.3.6 Test execution work products

Test execution work products bao gồm:

* Tài liệu về trạng thái của các test case riêng lẻ hoặc quy trình thử nghiệm (ví dụ: sẵn sàng để chạy, vượt qua, thất bại, bị chặn, bỏ qua có chủ ý, v.v.
* Báo cáo lỗi
* Tài liệu về (các) mục thử nghiệm, đối tượng thử nghiệm, công cụ kiểm thử và phần mềm kiểm thử đã tham gia và thử nghiệm.

#### **4.3.7** __ Test completion work products

Test completion work products bao gồm test summary report, các mục hành động để cải thiện dự án hoặc lặp lại tiếp, thay đổi yêu cầu hoặc các mục tồn đọng của sản phẩm và phần mềm kiểm thử đã hoàn thành.

### 4.4 Truy nguyên trong quá trình thử nghiệm giữa từng yếu tố của test basis và test work products

Để thực hiện giám sát và kiểm soát thử nghiệm hiệu quả, điều quan trọng là phải thiết lập và duy trì khả năng truy nguyên trong suốt quá trình thử nghiệm giữa từng yếu tố của test basis và test work products khác nhau được liên kết với yếu tố đó. Ngoài việc đánh giá phạm vi kiểm thử, việc truy nguyên cần hỗ trợ/đáp ứng các yêu cầu sau:

* Phân tích được tác động của những thay đổi
* Việc kiểm thử có thể kiểm thử đối chiếu và sửa chữa được
* Đáp ứng tiêu chí quản trị CNTT
* Cải thiện tính dễ hiểu của báo cáo tiến độ thử nghiệm và báo cáo tóm tắt thử nghiệm để bao gồm trạng thái của các yếu tố của cơ sở thử nghiệm (ví dụ: các yêu cầu đã vượt qua thử nghiệm của chúng, yêu cầu không vượt qua thử nghiệm và yêu cầu có thử nghiệm đang chờ xử lý).
* Liên quan đến các khía cạnh kỹ thuật của thử nghiệm với các bên liên quan theo các khía cạnh mà họ có thể hiểu
* Cung cấp thông tin để đánh giá chất lượng sản phẩm , khả năng xử lý và tiến độ dự án so với mục tiêu kinh doanh

Một số công cụ quản lý kiểm thử cung cấp các mô hình test work products khớp với một phần hoặc tất cả test work products được nêu trong phần này. Một số tổ chức xây dựng hệ thống quản lý riêng để tổ chức các sản phẩm công việc và cung cấp truy suất nguồn gốc thông tin mà họ yêu cầu.

## 5. Tâm lý trong testing

Phát triển phần mềm, bao gồm việc kiểm thử phần mềm có sự tham gia của con người. Vậy nên, tâm lý con người có ảnh hưởng quan trọng lên kiểm thử phần mềm.

### 5.1 Tâm lý của con người trong kiểm thử

Một yếu tố của tâm lý con người được gọi là comfirmation bias (thiên kiến xác nhận) có thể gây ra việc khó chấp nhận các thông tin ngược lại với niềm tin đang được nắm giữ.Cùng với thiên kiến xác nhận, các thiên kiến nhận thức (cognitive bias) khác cũng có thể là họ khó hiểu hay chấp nhận thông tin được đưa ra bởi testing. Xa hơn, một nét tính cách thông thường của con người là hay trách cứ người mang đến tin xấu, mà thông tin đưa đến sau khi test thường là các tin xấu. Kết quả của các nhân tố tâm lý trên là một số người có thể nhận thức rằng testing là một hành động phá hoại, mặc dù nó đóng góp rất nhiều vào tiến độ và chất lượng của dự án. Để giảm thiểu các nhận thức như vậy, thông tin về các defects và failures nên được góp ý có tính xây dựng. Theo cách này, sự căng thẳng giữa các testers và analysts, product owners, designers và developers có thể giảm đi. Điều này áp dụng cả trong static và dynamic testing. Tester và test managers cần có kĩ năng xây dựng mối quan hệ giữa cá nhân tốt, để có thể giao tiếp với nhau một cách hiệu quả vể các defects, failures, test results, test progress và risks. Các để giao tiếp tốt bao gồm những ví dụ sau:

* Bắt đầu bằng sự hợp tác hơn là tranh đấu. Nhắc nhở mọi người về những mục tiêu chung vể hệ thống có chất lượng tốt hơn
* Nhấn mạnh về lợi ích của testing. Ví dụ, cho những người viết requiement, thông tin về defect có thể giúp họ cải thiện work products và kĩ năng của họ. Cho tổ chức, các defects được tìm thấy và sửa trong quá trình testing sẽ giúp giảm thời gian, tiền bạc và giảm các rủi ro chung cho chất lượng product
* Thông tin về test results và các điều tìm thấy theo hướng trung lập, tập trung vào sự thật và tránh chỉ trích người tạo ra defect đó. Viết ra mục tiêu, report sai sót thực tế và xem lại những điều tìm thấy
* Cố gắng hiểu cảm nghĩ của người khác và lí do việc họ phản ứng một cách tiêu cực với thông tin
* Xác nhận rằng người nghe đã hiểu những gì mình nói và ngược lại

### 5.2 Tư duy của Tester và Dev

Developers và tester thường có cách nghĩ khác nhau. Mục tiêu cơ bản của việc phát triển phần mềm là thiết kế và xây dựng nên một sản phẩm. Mục tiêu của việc testing bao gồm kiểm tra và xác nhận (verifying and validating) sản phẩm, tìm các defects trước khi release… Có những tập mục tiêu khác nhau nên yêu cầu các mindsets khác nhau. Mang những mindset này lại với nhau giúp đạt được các mức độ cao hơn về chất lượng sản phẩm. Một mindset phản ánh một sự giả định mang tính cá nhân và những phương pháp ưa thích để đưa ra quyết định và xử lý vấn đề.

* Mindset của một tester nên bao gồm sự tò mò, sự bi quan, con mắt tinh tường, chú ý vào chi tiết, sự thúc đẩy làm điều tốt và khả năng giao tiếp và tạo dựng mối quan hệ tốt. Một mindset tester hướng tới sự phát triển và trưởng thành khi tester đó luôn tích cóp các kinh nghiệm.
* Mindset của một developer có thể bao gồm một vài điểm giống với mindset của tester, nhưng một developer thành công thường thích việc thiết kế và đưa ra giải pháp hơn là việc dự tính những điều sai sót có thể xảy ra với giải pháp đó. Hơn nữa, thiên kiến xác nhận gây khó khăn để có thể nhận ra được các lỗi tạo ra bởi chính họ.

Với một mindset đúng đắn, các developer hoàn toàn có thể test code của chính họ. Các mô hình phát triển phần mềm khác nhau thường có các cách khác nhau để quản lý các tester và các hoạt động test. Một vài hoạt động test được hoàn thành bởi các tester độc lập sẽ tăng hiểu quả trong việc phát hiện ra defect, phần mà đặc biệt quan trọng cho các hệ thống lớn, phức tạp và đặt an toàn lên hàng đầu (safety-critical). Các tester độc lập sẽ mang đến góc nhìn khác với góc nhìn của work product authors (như là business analysts, product owner, designers và developers), vì họ các thiên kiến nhận thức khác với các authors.
