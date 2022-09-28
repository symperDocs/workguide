---
description: Hướng dẫn sử dụng tool thiết kế
---

# Design Tool

## 1. Figma

### 1.1. Mục đích & lý do sử dụng

Figma là công cụ được sử dụng để tạo bản mockup và prototype cho Web/App. Là công cụ được ưu tiên sử dụng hàng đầu của các Designer kể cả các newbee&#x20;

Lý do sử dụng Figma :&#x20;

* Giao diện tối giản, thân thiện và dễ sử dụng
* &#x20;Có thể truy cập trên bất cứ hệ điều hành nào, hỗ trợ lưu trữ đám mây tiện lợi&#x20;
* Cho phép chia sẻ, mời người dùng khác dễ dàng và có thể comment trực tiếp trên project đang thực hiện

### 1.2. Cách sử dụng

#### 1.2.1. Cách tạo mới

* _**Tạo team mới:**_&#x20;

Để tạo team mới trước hết bạn cần có tài khoản Figma và đăng nhập sử dụng thành công. Ngay màn hình giao diện ban đầu, dưới góc trái của sidebar , bạn click vào + Create new team. Tiếp tới là điền các thông tin như Tên của team, thêm thành viên trong team và lựa chọn chi phí sử dụng (bạn có thể chọn Starter để bắt đầu miễn phí với một số giới hạn nhất định)

![Thêm mới team](<.gitbook/assets/image (38) (1) (1) (1).png>)

* _**Tạo file thiết kế mới:**_&#x20;

Trong team mới vừa tạo, có ngay một project tên Team project, bạn có thể thao tác với project bằng cách chuột phải vào Team project.&#x20;

**Các hành động với project bao gồm:**&#x20;

\-Share New design file (Thêm mới file thiết kế figma)&#x20;

\-New Figjam file (Thêm mới bảng trắng Figjam)&#x20;

\-Rename Remove from favorites&#x20;

\-Delete&#x20;

Click vào New design file để tạo mới file, hoặc Click vào thẻ New design file trên màn hình chính giữa, một giao diện thiết kế sẽ được mở ra cho bạn thực hiện.

![Thao tác thêm mới file](<.gitbook/assets/image (27) (1).png>)

**1.2.2. Các tính năng chính của Figma**

Các phần mềm thiết kế nói chung và Figma nói riêng sẽ có rất nhiều các tính năng phục vụ cho việc thiết kế, trong phạm vi hướng dẫn này sẽ tập trung chủ yếu vào một vài những tính năng chính và nổi bật designer cần nắm được để thao tác cơ bản với Figma

Trước hết, một màn hình Figma khi bắt đầu project bao gồm các thành phần:

![Các thành phần trong màn hình vẽ](<.gitbook/assets/image (38) (1) (1).png>)

1 - Menu bar\
2- Tên project/ Tên file thiết kế\
3- Tổng hợp các layout và component có trong bản vẽ\
4- Thông tin tài khoản, share link, % man hình hiển thị, run flow của prototype\
5- Khu vực config của mockup, prototype và inspect\
6- Khu vực thực hiện vẽ

Dưới đây là một số các tính năng chính khi thao tác với Figma

* _**Di chuyển kéo thả**_

![Thao tác di chuyển](<.gitbook/assets/image (24).png>)

* _**Vẽ frame**_

![Thao tác vẽ frame](<.gitbook/assets/image (30) (1).png>)

Sau khi vẽ frame, bạn chỉnh sửa các thông số tại sidebar bên phải.&#x20;

![Các thuộc tính của frame](<.gitbook/assets/image (39) (1).png>)

**Các thuộc tính của frame bao gồm:**\
1- Align\
2- Tọa độ\
3- Chiều cao, chiều rộng \
4- Góc xoay và bo góc\
5- Auto Layout\
6- Layout grid\
7- Độ trong suốt\
8- Tô màu toàn bộ\
10- Stoke: viền\
11- Effects: Đổ bóng\
12- Export: Xuất frame

* _**Vẽ hình khối**_

![Thao tác vẽ hình khối](<.gitbook/assets/image (37) (1).png>)

Các thuộc tính của một hình khối cũng giống với các thuộc tính của frame như đã nêu ở trên

![Thuộc tính của các hình khối](<.gitbook/assets/image (37).png>)

* _**Taọ nhóm**_

Bạn nhấn giữ shift + click chọn các đối tượng cần gom nhóm hoặc bôi đen toàn bộ các đối tượng đó, sau đó chuột phải chọn Group selection hoặc phím tắt Ctrl+G(window)

![Thao tác tạo nhóm](<.gitbook/assets/image (31).png>)

Frame cũng là một nhóm bao gồm các thành phần, tuy nhiên frame khác group ở chỗ khi phóng to thu nhỏ, các thành phần bên trong sẽ không thay đổi kích thước mà chạy theo lễ của frame. Trong khi đó kích thước của các đối tượng trong group sẽ bị thay đổi (theo cơ chế vector).

* _**Tạo component(compo)**_

Bạn có thể lựa chọn 1 group, 1 frame hay thậm chí là 1 hình khối...để tạo 1 compo có thể tái sử dụng lại. Lợi ích của việc tạo compo còn là việc chỉnh sửa nhanh nhiều đối tượng cùng 1 lúc, khi mà chỉ cần chỉnh sửa compo chính, các compo con sẽ bị thay đổi theo.\
\
Ngược lại khi bạn sửa 1 compo con, sẽ không ảnh hưởng đến compo chính và các compo con khác. Lúc này nếu thay đổi compo cha thì chỉ ảnh hưởng đến compo con chưa chỉnh sửa. \
\
Nếu muốn compo con vừa sửa trở lại format ban đầu như compo cha, bạn chuột phải vào compo hoặc click thuộc tính của compo bên sidebar chọn Reset all overrides.

![Các phần tử component](<.gitbook/assets/image (25) (1).png>)

* _**Auto Layout**_

Đây là kỹ thuật rất hữu ích khi thiết kế với Figma giúp designer tiết kiệm được nhiều công sức và thời gian thiết kế.\
Auto-layout giúp bạn tạo ra một layout hoặc component tự động điều chỉnh thay đổi kích thước theo sự thay đổi của nội dung bên trong hoặc của đối tượng chứa bên ngoài.

Khi chúng ta cần thêm hay bỏ bớt một thành phần trong layout, toàn bộ các thành phần còn lại sẽ được tự động được thay đổi theo cho phù hợp, không cần tốn nhiều thao tác thủ công để sắp xếp, điều chỉnh lại. Tính năng này sẽ rất hữu ích khi bạn cần thiết kế giao diện cho nhiều kích cỡ màn hình của các thiết bị khác nhau.\
\
**Cách thực hiện:** \
\- Từ hình trên, ta đang có 3 hình elip với khoảng cách chưa được căn chỉnh. Bạn chọn cả 3 elip, nhấn phím tắt Shift+A , các hình sẽ lập tức được nhóm lại thành 1 frame và được align theo hàng ngang.\
\- Các thuộc tính của Auto Layout trong side bar lần lượt gồm sắp xếp theo chiều dọc, sắp xếp theo chiều ngang, khoảng cách giữa các phần tử, auto pading, pading từng cạnh.

![Config auto layout](<.gitbook/assets/image (38) (1).png>)

\-Khi thêm hoặc bớt bất kỳ phần tử nào trong frame thì các phần tử còn lại sẽ tự động được sắp xếp theo đúng với các thông số đã config.

![Thêm phần tử vào auto layout](<.gitbook/assets/image (39).png>)

* _**Xử lý hình ảnh**_

Để cắt ảnh theo hình mong muốn, bạn sử dụng tính năng Use as mask trong menu chuột phải. Thao tác thực hiện:\
B1 - Tạo 1 hình khối mà bạn muốn cắt ảnh theo\
B2 - Xếp hình khối lên trên khu vực ảnh mà bạn muốn cắt&#x20;

![Thao tác thêm hình khối](<.gitbook/assets/image (41).png>)

B3- click chuột phải chọn Use as mask .Kết quả sẽ thu được hình ảnh được cắt theo khuôn mong muốn\


![Chọn Use as mask để cắt ảnh](<.gitbook/assets/image (25).png>)

![Ảnh sau khi dùng use as mark](<.gitbook/assets/image (42) (1).png>)

* Viết /vẽ tay

![Công cụ viết/vẽ tay](<.gitbook/assets/image (35).png>)

**1.2.3. Các quy tắc Design system khi thiết kế bằng Figma**

* Quy tắc đặt tên màn hình:

Designer cần thực hiện đặt tên cho từng màn hình trong bản thiết kế nhằm tạo cách gọi chung cho các bên thực hiện sản phẩm như BA, Dev, Des và QC, giúp tăng hiệu quả trong giao tiếp, trao đổi về sản phẩm.

Việc đặt tên màn hình có các quy định như sau:

\-Ngắn gọn và đủ nội dung

\-Thể hiện được thao tác/tính năng được vẽ trong màn hình.

Ví dụ: Thao tác thêm bản ghi hay sửa, xóa thì tên màn hình cần ghi rõ thao tác đó

\-Thể hiện được đối tượng sử dụng thao tác/tính năng được vẽ trong màn hình

Ví dụ: Đối tượng sử dụng là BA thì tên màn hình sẽ là BA-Thêm bản ghi, là End-user thì sẽ là EU-Thêm bản ghi

\-Các màn hình cùng thể hiện một đối tượng sử dụng hoặc một thao tác/tính năng sẽ được đặt kèm theo số tịnh tiến theo trình tự thực hiện thao tác.&#x20;

Ví dụ: 06 màn hình đều là BA-Thêm bản ghi thì sẽ lần lượt là BA-Thêm bản ghi 1, BA-Thêm bản ghi 2,...BA-Thêm bản ghi 6 .

* Quy tắc đặt tên group:

Việc đặt tên cho các group hay các frame cũng là một cách để tạo cách gọi chung trong giao tiếp giữa các bên thực hiện sản phẩm nhưng ở mức độ chi tiết hơn.

Designer đặt tên cho các frame thể hiện nội dung chính màn hình, các frame này có thể là các component hoặc một nhóm các component.

Ví dụ: Trong màn hình BA- Thêm bản ghi thì pop-up nhập nội dung bản ghi là một nhóm component thể hiện nội dung chính của màn hình nên cần đặt tên.

Quy định đặt tên group tương tự như đặt tên màn hình.

* Quy tắc 4pt grid

Theo Design System, hệ thống 4pt grid áp dụng giúp designer và dev dễ dàng trong việc căn chỉnh các thành phần trong màn hình. Do vậy việc áp dụng hệ thống 4pt grid là một trong những quy tắc bắt buộc trong thiết kế.&#x20;

Designer áp dụng hệ thống 4pt bằng cách căn độ rộng, chiều cao, khoảng cách... các thành phần với công sai 4pt( hay sử dụng bội số của 4: 4,8,12,16...)

* Quy tắc sử dụng màu:

Ngoài các nhóm màu được liệt kê trong Design System thì khi Designer lựa chọn màu sẽ cần tuân thủ theo một số quy tắc sau:

\-Về mục đích sử dụng: Mỗi màu sắc thể hiện một trạng thái khác nhau đem đến cảm xúc khác nhau cho người dùng . Ví dụ như màu đỏ thường là sự nổi bật, sự nguy hiểm. Do đó thường dùng màu đỏ cho các thông báo lỗi, xóa bỏ đối tượng. Màu xanh lá cây thường là sự sinh sôi, nhân lên về số lượng...nên được dùng cho các button Lưu, Thêm mới hoặc các thông báo thành công.

Trên hệ thống Symper hiện tại sử dụng 4 màu chính:

![](<.gitbook/assets/image (24) (1).png>)dùng cho các button, layout, container, text...của hệ thống

![](<.gitbook/assets/image (41) (1).png>) dùng cho các button, hyperlink, tab... quan trọng, sử dụng xuyên suốt để nhấn mạnh màu thương hiệu của hệ thống

![](<.gitbook/assets/image (42) (1) (1).png>) dùng cho button, dialog...mang ý nghĩa lưu, áp dụng, thông báo thành công

![](<.gitbook/assets/image (25) (1) (1).png>) dùng cho button, dialog...mang ý nghĩa báo lỗi, cảnh báo bắt buộc, xóa bỏ...

Ngoài ra có thể sử dụng thêm màu xanh #346DDB để thể hiện thông tin mở rộng, nguyên nhân, cách khắc phục...

\-Về độ tương phản: quy tắc này tương đồng với Text Legibility trong Design System tuy nhiên mở rộng hơn với cách sử dụng màu cho các phần tử khác trong hệ thống.&#x20;

Màu tương phản có tác dụng phân tách các thành phần trong một giao diện và thu hút sự chú ý của người dùng vào các thành phần được làm nổi bật. Điều chỉnh độ đậm nhạt cũng là một cách để tăng tính tương phản giữa các đối tượng. Tuy nhiên trong cùng một component, designer cần cân nhắc dùng màu nóng kết hợp với màu lạnh.

**1.2.4. Thao tác tạo prototype**

### **1.3. Lưu ý khi sử dụng**

* Designer có thể thêm ghi chú ngay cạnh các trang thiết kế để note lại thao tác hoặc req giúp các bên tiếp nhận bản thiết kế có thể theo dõi dễ hơn và không bị sót các req.
* Khi thiết kế, ngoài việc tuân thủ các quy tắc trên và quy tắc Design System, designer nên áp dụng kỹ thuật Auto Layout và tính năng Creat Component giúp giảm thời gian và đồng nhất được thiết kế.

## **2.ADOBE XD**

### **2**.1. Mục đích & lý do sử dụng

### 2.2. Ưu nhược điểm&#x20;
