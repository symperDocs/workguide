---
description: Hoanp
---

# CREATE FUNCTION FORMULA

Hàm Create function dùng để tạo ra một function mới trên hệ thống. Nhìn vào ví dụ dưới đây:

> ref(DROP FUNCTION IF EXISTS user\_name(character varying);
>
> CREATE FUNCTION user\_name(user\_id character varying)
>
> RETURNS TABLE(user\_name TEXT)
>
> language plpgsql AS
>
> \$$
>
> BEGIN
>
> RETURN QUERY
>
> select display\_name from users where id = user\_id;
>
> END;
>
> \$$;

* Hàm Drop function if exist: dùng để xoá bỏ function user\_name nếu trên hệ thống đã tồn tại function này. Điều này nhằm đảm bảo không có 2 function trùng tên cùng tồn tại.
* Hàm Create function: tạo ra function tên "user\__name"_ với giá trị đầu vào là cột dữ liệu "user\_id" với kiểu dữ liệu là character varying. Function này sẽ trả ra table gồm 1 cột tên là user\_name và kiểu dữ liệu là TEXT, ngôn ngữ plpsql
* Cấu trúc của function bắt đầu từ \$$ BEGIN RETURN QUERY và kết thúc tại END \$$. Nội dung sau RETURN QUERY sẽ là cấu trúc của function mà bạn đang tại, và kết quả đầu ra của query sẽ được đổ về table trước đó.
