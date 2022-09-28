---
description: n8n
---

# Intergration

## Mục đích&#x20;

Hướng dẫn sử dụng quy trình của n8n để thêm bản ghi mới vào doc service version trên inter khi release version mới trên github

## Logic

Khi thực hiện release version trên github, n8n lấy api từ github kèm theo các thông tin version code, title, mô tả, thời gian release,.... để thực hiện insert vào Document của Symper

![Chi tiết quy trình](<.gitbook/assets/image (59).png>)

Để lấy được thông tin từ github symper thì cần có Access Token, Repo Owner, Repo Name

![Github Trigger](<.gitbook/assets/image (20).png>)

Tiếp theo n8n sẽ xử lý phần dữ liệu để có thể insert đúng định dạng Document của Symper, bao gồm việc lấy các thông tin, chuyển đổi kiểu dữ liệu, lọc dữ liệu cần thiết, insert theo cấu trúc của control, table,...

![Workflow](<.gitbook/assets/image (56).png>)

{% hint style="info" %}
[Workflow](http://n8n-test.symper.vn:5667/workflow/12)
{% endhint %}

Cấu trúc insert dữ liệu vào doc ở node ![](<.gitbook/assets/image (72).png>) trong workflow

![Expression](<.gitbook/assets/image (42).png>)

## Đối tượng sử dụng

### Dev

Cần nắm rõ các thông tin khi release code sẽ được insert vào control nào trong doc

![Github](<.gitbook/assets/image (49).png>)

Chú ý: Dữ liệu chỉ được insert vào document khi dev nhấn vào publish release

![Symper](<.gitbook/assets/image (99).png>)

Quy tắc điền phần mô tả

* Đối với REQ và BUG thì phải điền theo quy tắc TYPE\_ID_DES (Theo thứ tự type -> id -> des và giữa các trường thông tin phải có dấu gạch dưới_ "_\__") Bắt buộc

{% hint style="info" %}
ISS\_ISS2204121_\__Kanban end user
{% endhint %}

* Sau khi kết thúc thì xuống dòng và lặp lại quy tắc trên cho REQ hoặc BUG mới
* Đối với những nội dung không phải là REQ hoặc BUG thì chỉ cần điền nội dung chính

{% hint style="info" %}
Cải thiện performance phần BI
{% endhint %}

_Ex_

![Mô tả](<.gitbook/assets/image (88).png>)
