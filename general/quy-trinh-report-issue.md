# Quy trình report issue

## Nhu cầu

Trong quá trình triển khai, việc thống kê và trao đổi các vấn đề phát sinh như bug, requirement là rất cần thiết.

Module hỗ trợ triển khai phục vụ giúp BA trở thành bộ lọc các vấn đề trước khi đẩy về team phát triển sản phẩm.

## Các issue phát sinh

Trong quá trình triển khai sẽ có một số các trường hợp sau phát sinh từ phía khách hàng:

* Các bug phát sinh trong quá trình sử dụng hệ thống
* Nhu cầu về thay đổi thông tin
* Nhu cầu giải đáp các vấn đề về tính năng trong quá trình sử dụng
* Nhu cầu về bổ sung tính năng phía hệ thống

## Case study

Thống kê các issue cần thiết có một document để người dùng và BA tương tác, trao đổi, chốt vấn đề.

Ví dụ: Với ứng dụng QC của Symper

<figure><img src="../.gitbook/assets/image (32) (1) (1).png" alt=""><figcaption><p>Màn hình doc khai báo issue của Symper</p></figcaption></figure>

<figure><img src="../.gitbook/assets/image (30) (1) (1).png" alt=""><figcaption></figcaption></figure>

## Phương án

### Document:

Mô tả luồng kế thừa và thiết kế của doc khai báo issue:

<figure><img src="../.gitbook/assets/image (6) (2).png" alt=""><figcaption></figcaption></figure>

### Workflow:

Quy trình báo cáo và tiếp nhận issue tại

<figure><img src="../.gitbook/assets/image (37) (1).png" alt=""><figcaption></figcaption></figure>

### Data

Đây là một số ví dụ về việc chia nhóm data, khi triển khai sẽ liệt kê chi tiết hơn các dữ liệu phân nhóm này.

**Nhóm vấn đề**

| Mã nhóm | Tên nhóm                        |
| ------- | ------------------------------- |
| DOC01   | Lỗi khi submit văn bản          |
| DOC02   | Lỗi khi in văn bản              |
| DOC03   | Lỗi khi xem văn                 |
| WF01    | Lỗi thực hiện phê duyệt task    |
| WF02    | Lỗi khi xem task detail         |
| BI01    | Lỗi khi xem chi tiết báo cáo    |
| BI02    | Lỗi khi in báo cáo              |
| BI03    | Lỗi khi filter dữ liệu trên báo |

### Hành động:

| Mã nhóm | Mã hành động | Tên hành động                  |
| ------- | ------------ | ------------------------------ |
| DOC01   | DOC01-AC001  | Lỗi khi nhập liệu và input có  |
| DOC01   | DOC01-AC002  | Lỗi thêm, xoá dòng trong table |
| DOC01   | DOC01-AC003  | Lỗi nhập liệu trong cell       |

### Nguyên nhân phát sinh:

| Mã nguyên nhân | Tên nguyên nhân                      |
| -------------- | ------------------------------------ |
| PR001          | Nguyên nhân thao tác của người       |
| PR002          | Người dùng chưa biết cách sử dụng hệ |
| PR003          | Lỗi giao diện người dùng             |
| PR004          | Lỗi dữ liệu hệ                       |
| PR005          | Lỗi config                           |
