---
description: Reposted by Huongntm
---

# Chuẩn hoá và phân loại doc

## TRƯỚC KHI XÂY DỰNG ỨNG DỤNG

* Luôn phác thảo ý tưởng doc/quy trình/luồng xử lý dữ liệu/ báo cáo ra và được phê duyệt trước mới tiến hành thực hiện&#x20;
* Khi chỉnh sửa các ứng dụng đã được dựng rồi thì bất cứ thay đổi về các thông tin trong ứng dụng hay bổ sung/xóa bớt các đối tượng đều phải hỏi ý kiến project manager của dự án đó.&#x20;

## **CHUẨN HÓA VÀ PHÂN LOẠI DOCUMENT** <a href="#chuan_hoa_va_phan_loai_document" id="chuan_hoa_va_phan_loai_document"></a>

### **Phân loại Doc** <a href="#phan_loai_doc" id="phan_loai_doc"></a>

Phân loại các Smart Doc được chia như sau:

* Nhóm **Doc danh mục**: danh mục là các Doc chứa thông tin khởi tạo, cung cấp thông tin cho các Doc nghiệp vụ (ví dụ: danh mục hàng hóa, danh mục kho, danh mục đối tác .....). Doc danh mục không nằm trong các Workflow (= không tham gia trực tiếp, nhưng có thể được tham chiếu tới).
* Nhóm **Doc nghiệp vụ**: là các Doc phục vụ cho các module nghiệp vụ và luân chuyển trong các Workflow từ User này sang user kia, và mang thông tin của từng giao dịch (= transaction). 2 loại Doc nghiệp vụ: (i) Doc nghiệp vụ chính (là Doc chắc chắn có ở bất kỳ khách hàng, loại hình kinh doanh nào); và (ii) Doc nghiệp vụ phụ (là các Doc có thể có có thể không) --> ví dụ: Hóa đơn, Đơn hàng, Phiếu nhập mua là các Doc nghiệp vụ chính, nhưng Thông báo nhập kho, Phiếu Giao việc là các Doc nghiệp vụ phụ;
* Nhóm Doc xử lý: là các Doc sinh ra ngoài 2 mục đích ở trên (thường dùng cho BA trong các mục đích cập nhật thông tin ở các Doc danh mục or Doc nghiệp vụ cho mục đích xử lý các tình huống ....) -> Doc này nếu xử lý tốt, thì không nên có --> số lượng các Doc này nên hạn chế, dùng xong nếu không có ý định dùng tiếp thì cần xóa đi.

### **Phân nhóm các Doc** <a href="#phan_nhom_cac_doc" id="phan_nhom_cac_doc"></a>

Các Smart Doc ngoài phân loại, thì được phân nhóm vào các Modules nghiệp vụ:

* Module Nghiệp vụ: bao gồm các Doc danh mục của Modu
* Module Hệ thống: bao gồm cac Doc danh mục hệ thống;
* le, và Doc nghiệp vụ của Module (Module nghiệp vụ có thể kể tới như Mua hàng, Bán hàng, ....) -> có trường hợp 1 Doc danh mục hoặc nghiệp vụ sẽ phục vụ nhiều module.
* Doc danh mục

### **Cách đặt tên và tiêu đề Doc** <a href="#cach_dat_ten_doc" id="cach_dat_ten_doc"></a>

* Font chữ mặc định: ROBOTO
* Size của Title Doc: **18 ptx, Bold, màu cam**
* Size chữ trong Body của Doc: **13 ptx, màu đen**
* Size chữ của Title section\*\*: 14 ptx, Bold, màu cam\*\*

**Tên doc**

* Doc danh mục luôn bắt đầu với "dm" + '\_" + "tên danh mục" -> ví dụ: Danh mục hàng hóa dịch vụ ->vang dm\_hhdv
* Doc nghiệp vụ = "tên viết tắt module" + "\_" + "tên nghiệp vụ" -> ví dụ: Phiếu nhập mua -> "pu\_pnm"
* Tên doc được giới hạn ở 12 ký tự → ví dụ: dm\_kho\_hang là 11 ký tự.
* Không viết hoa, không viết liền
* Quy tắc mã danh mục hệ thống: [https://docs.google.com/spreadsheets/d/1oTmW1wcCtZtem53msbK7ZOWUVwV771gyry47paqBOVc/edit#gid=1372855654](https://docs.google.com/spreadsheets/d/1oTmW1wcCtZtem53msbK7ZOWUVwV771gyry47paqBOVc/edit#gid=1372855654)

**Tiêu đề doc**

* Tiêu đề doc có dạng: \[ mã biểu mẫu ] + 'tên rút gọn doc" .-> ví dụ : \[BM.04.05] PKTRA CLG ĐVÀO NL XƯƠNG

Trong đó mã biểu mẫu thường được quy định trong quy trình, các doc có thể có hoặc không có mã biểu mẫu.

Tiêu đề doc không vượt quá 30 ký tự , viết IN HOA và rút gọn các trường thông tin theo tiêu đề control

Cụ thể rút gọn:

* SỔ THEO DÕI = SỔ TD
* SỔ GIAO CA = SỔ G.CA
* PHIẾU KIỂM TRA = PKT
* SỔ TỔNG HỢP = SỔ TH
* DANH MỤC = DM
* YÊU CẦU = YC
* KHAI BÁO = KB

Lưu ý:

* Các **Doc danh mục, Doc nghiệp vụ chính** (cả tên Doc, tên control và table trong doc) -> cần được chuẩn hóa, phục vụ việc pack các Module, và đảm bảo các công thức chạy;
* Các Doc nghiệp vụ phụ -> các **Control hệ thống** (đã được chuẩn hóa cách đặt) của các Doc nghiệp vụ phụ này cũng cần được chuẩn hóa -> chỉ có các control không được chuẩn hóa thì người đặt phải tuân theo **NAMING CONVENTION** của **SYMPER**

**Cách cấu hình layout doc**

* Nếu trong table có nhiều hơn 2 table thì có thể sử dụng control tab & page để chứa các table (mối table có thể nằm trong 1 tab hoặc 1 page)
* Phần thông tin chung của doc phải được sắp xếp trong table layout để căn chỉnh thẳng hàng và chính xác

**Cấu hình thuộc tính chung của doc**

* Chọn loại văn bản
* Thông tin ghi chú (sử dụng để hiển thị trong module search)
* Tiêu đề bản ghi (dùng để hiển thị trong my item, BA có thể sử dụng SYQL để tạo ra phần hiển thị này)

**Cấu hình các trường dữ liệu trong doc**

| **STT** | **Các mục cần phải config của control trong document**                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| ------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1       | <p>Số chứng từ (nếu có) phải có cấu hình tự tạo ra số chứng từ (Sử dụng <strong>control primary</strong>)</p><p>- Sử dụng mã chứng từ và ngày chứng từ để tạo số chứng từ (Cấu tạo SCT = &#x3C;Mã công ty>/&#x3C;Mã CT>&#x3C;Số thứ tự (4 số)></p><p><em>Ví dụ CVN/UA22070001</em>)</p><p>- Cập nhật tăng số chứng từ vào doc danh mục quyển chứng từ</p><p>- Validate số chứng từ (tránh trùng)</p><p>- Check vào thuộc tính định danh để đảm bảo không xảy ra trường hợp trùng số chứng từ - Check vào thuộc tính required để đảm bảo phải điền số chứng từ</p> |
| 2       | Ghi chú: tự động tạo ra thông tin của trường ghi chú. Các trường thông tin ghi chú phải căn chiều rộng ít nhất 500px để hiển thị được nhiều thông tin hoặc tuỳ vào layout mà để max độ rộng nếu có thể                                                                                                                                                                                                                                                                                                                                                            |
| 3       | Các control có auto complete thì phải có validate dữ liệu nhập vào nếu như không cho phép điền sai thông tin                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 4       | Đối với danh sách cho user chọn mà không có việc tăng thêm về mặt dữ liệu (danh sách fix cứng) thì sử dụng control select                                                                                                                                                                                                                                                                                                                                                                                                                                         |
| 5       | Doc có các trường thông tin về người nếu lấy từ danh sách user của hệ thống thì phải dùng control user                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 6       | Các trường number phải đảm bảo format định dạng có phần thập phân nếu như các trường đấy không phải số nguyên và có phân lớp phần nghìn: Định dạng mặc định phân lớp phần nghìn và 2 ký tự thập phân sau dấu "."                                                                                                                                                                                                                                                                                                                                                  |
| 7       | Các trường number phải có validate không cho phép nhập âm (không bắt buộc vì có thể có trường được phép nhập âm)                                                                                                                                                                                                                                                                                                                                                                                                                                                  |
| 8       | Bắt buộc có "Approval History" Control ở các Document tham gia vào Workflow (Doc Nghiệp vụ)                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 9       | Khi tạo document bắt buộc phải nhập liệu vào trường thông tin Tiêu đề bản ghi trong thuộc tính của document                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 10      | Bỏ thuộc tính quan trọng của control nếu không thực sự cần thiết, chỉ giữ lại nhiều nhất 13 control quan trọng để được hiển thị lên showlist                                                                                                                                                                                                                                                                                                                                                                                                                      |

**Cấu hình form in của doc**

* Cấu hình form in mặc định size A4
* Font chữ Time new roman (size 13px)
* Nếu table trong doc có quá nhiều trường thông tin thì xem xét quay ngang khổ giấy của form in
* Loại bỏ bớt các trường thông tin không cần thiết để in

## **CHUẨN HÓA VÀ PHÂN LOẠI TABLE** <a href="#chuan_hoa_va_phan_loai_table" id="chuan_hoa_va_phan_loai_table"></a>

Phân loại table

* Table hệ thống: là table nằm trong các: (i) Doc Danh mục, và (ii) Doc nghiệp vụ chính.
* Table sự vụ: ngoài các Table hệ thống, và có thể nằm trong các Doc Danh mục và Doc nghiệp vụ chính, trong trường hợp là các Table tạo thêm, đặc thù cho khách hàng đó.

Các control bảng cần được đặt tên:

* Tên bảng = tbx (x tịnh tiến từ 1 tới n tùy theo thứ tự khởi tạo của bảng)
* Tiêu đề của bảng = xxxx (xxxx phải mô tả được nội dung của bảng để làm gì -> xem các convention đặt tên dưới đây);

Chuẩn hóa các Bảng trong các:

* Doc danh mục; và
* Doc nghiệp vụ chính

## **CHUẨN HÓA VÀ PHÂN LOẠI CONTROL** <a href="#chuan_hoa_va_phan_loai_control" id="chuan_hoa_va_phan_loai_control"></a>

### **Phân loại các Control** <a href="#phan_loai_cac_control" id="phan_loai_cac_control"></a>

* **Control trong hệ thống:** là các control nằm trong hệ thống chuẩn hóa tên dưới đây, đã được đặt tên trước (ví dụ: tên hàng, mã hàng, tên khách, mã khách, thuế suất, tiền trước thuế gtgt, tiền sau thuế gtgt, tiền nguyên tệ, giá ....); -> Cần follow chặt chẽ cách đặt tên control hệ thống này để đảm bảo việc công thức chạy
* **Control sự vụ:** là các control ít xuất hiện, và nằm ngoài các control hệ thống dưới đây.

### **Cách đặt tên và tiêu đề các control** <a href="#cach_dat_ten_cac_control" id="cach_dat_ten_cac_control"></a>

* Các tên control được chuẩn hóa cho 1 doc như sau (số ký tự của **tên control** không vượt quá **12** ký tự, **tiêu đề control** không vượt quá **16 ký tự**):
* Các control về là số tiền, thành tiền, trước thuế, sau thuế → luôn bắt đầu bằng "tien" (trừ trường hợp nằm trong table, thì bắt đầu sau tên control table). Ví dụ: thành tiền trước thuế = tien\_tt\_tt; thành tiền sau thuế = tien\_tt\_st; tiền thuế = tien\_thue
* Các control về số lượng, luôn bắt đầu bằng "sl", số lượng nhập kho = sl\_nk, số lượng xuất kho = sl\_xk, số lượng trình duyệt mua hàng = sl\_tdmh;
* Các control ngày (trừ ngày chứng từ \~ "nct" của chính Doc đó) luôn bắt đầu bằng "ngay\_"+"mô tả ngắn gọn";
* Các trường hợp phải dùng mã, tên đối tượng của nhà cung cấp, khách hàng, người nhận tiền .... đều dùng ma\_khach và ten\_khach
* Không viết hoa, không viết liền

Cụ thể như sau:

#### **Tên nhóm Control thông tin chung của Doc** <a href="#nhom_control_thong_tin_chung_cua_doc" id="nhom_control_thong_tin_chung_cua_doc"></a>

* Mã Công ty = ma\_cty và Tên Công ty = ten\_cty (Công ty là đối tượng chủ sở hữu của Giao dịch -> ví dụ Hóa đơn bán hàng do Cty Dekko xuất thì Cty Dekko chính là cty)
*   Số chứng từ = sct (Cấu tạo SCT = \<Mã công ty>/\<Mã CT>\<Số thứ tự (4 số)>

    _Ví dụ CVN/UA22070001_); Mã quyển chứng từ = smct; Số hiện tại: sht; Ngày chứng từ = nct; Trạng thái chứng từ = ttct; Trạng thái hạch toán = ttht; Số trạng thái chứng từ: ttct\_no, Tên chứng từ = tct, Trạng thái thanh toán = tttt, Mã chứng từ = mct, Tên chứng từ = tct
* Mã khách = ma\_khach, và Tên khách = ten\_khach (Áp dụng cho cả khách hàng, nhà cung cấp, cơ quan thuế, đơn vị cho vay, nhân viên trong trường hợp Tạm ứng/ Đề nghị thanh toán ....)
* Diễn giải = dien\_giai (áp dụng cho ngoài table), còn phần ghi chú chỉ xuất hiện trong table ở cột cuối, Ghi chú = ghi\_chu (nếu như có nhiều ghi chú trong doc thì đánh số tịnh tiến: ghi\_chu\_1, ghi\_chu\_2...

#### **Tên nhóm Control liên quan tới Kho/ HHDV** <a href="#nhom_control_lien_quan_toi_kho-_hhdv" id="nhom_control_lien_quan_toi_kho-_hhdv"></a>

* Mã hàng = ma\_hang (áp dụng cho tất cả các items cần mã như mã hàng hóa, dịch vụ, mã phí .......)\\
* Tên hàng = ten\_hang (áp dụng cho tất cả các items cần mã như mã hàng hóa, dịch vụ, mã phí .......)\\
* Kiểu hàng hóa dịch vụ = kieu\_hhdv —> ví dụ: dịch vụ, thành phẩm, bán thành phẩm, vật tư ....
* Mã kho = ma\_kho (nếu như có nhiều kiểu mã kho có thể thêm hậụ tố để phân biệt: ví dụ: Mã kho xuất: ma\_kho\_xuat, Mã kho nhập: ma\_kho\_nhap) và Tên kho = ten\_kho (thêm hậu tố để phân biệt như đối với mã kho)
* Tài khoản kế toán = tk (thêm hậu tố để phân biệt ví dụ: tài khoản kho = tk\_kho...) và Tên tài khoản = ten\_tk (thêm hậu tố tương tự tài khoản kế toán)
* Tài khoản kho = tk\_kho, Tên tài khoản kho = ten\_tk\_kho
* Tài khoản thuế = tk\_thue
* Tài khoản đối ứng = tk\_du
* Nhóm ngành = nhom\_nganh, Tên nhóm ngành = ten\_nhom\_nganh → dùng với là hoặc Profit Center hoặc Segment (Segment là mẹ của Profit Center)
* Mã công đoạn = ma\_cdgt, Tên công đoạn = ten\_cdgt
* Mã đơn vị nội bộ = ma\_dvnb ( = đơn vị nội bộ), Tên đơn vị nội bộ = ten\_dvnb, Nhóm đơn vị = nhom\_dv
* Usert ID (control user): user\_id, Tên user = ten\_user, Ảnh nhân viên = user\_pic
* Cấp bậc user = cb, Id của cấp bậc = cb\_id
* Mã số thuế = mst, Kiểu đối tác = kieu\_doi\_tac, Địa chỉ = dia\_chi
* Cục thuế = cuc\_thue
* Trạng thái sử dụng (1 - sử dụng; 0 - không sử dụng. Thường được sử dụng với control select) = ttsd
* Người đề nghị = nguoi\_dn (dùng cho phiếu nhu cầu mua, yêu cầu lĩnh vật tư, đề nghị nhập kho, đề nghị hoàn ứng/tạm ứng/thanh toán),Bộ phận (Bộ phận chung chung) = bp, Bộ phận đề nghị = bp\_dn, Bộ phận mua hàng = bp\_mh
* Dư nợ = tien\_du\_no (số tiền luôn bắt đầu bằng tiền)
* Nội dung tạm ứng,/ lý do thanh toán = nd\_tu → đổi sang **dien\_giai**
* Số chứng từ (liên quan tới doc) = "so\_"+"tên doc đó" → ví dụ: so\_tdmh (số tdmh), hoặc so\_dxctnb, Ngày chứng từ (liên quan tới Doc) = "ngay\_" + "tên Doc đó" → ví dụ: ngay\_dxctnb là ngày của dxctnb; hoặc ngay\_tdmh (ngày trình duyệt mua hàng).
* Bộ phận đề xuất = ngay\_ctkt
* Sô tiền tạm ứng = tien\_tam\_ung, Số tiền tạm ứng bằng chữ = tien\_tam\_ung\_bc
* Tiền nhận/ Tiền nhận được/ Tiền thu được/Tiền phải thu, tiền thu = tien\_nhan
* Phương thức tạm ứng/ thanh toán = pt\_tt
* Đối tượng nhận = ten\_khach,
* Số tài khoản ngân hàng = tknh\_so, Mở tại ngân hàng = tknh\_ngan\_hang
* Ngày yêu cầu ứng = ngay\_ychu, Ngày hoàn ứng dự kiến = ngay\_hudk
* Ngày tạm ứng = ngay\_tam\_ung
* Số thực chi = tien\_ung\_tt (tiền ứng thực tế)
* Ngày hoàn thiện = ngay\_htcv (ngày hoàn thành công việc)
* Ngày hoàn ứng = ngay\_hoan\_ung
* Dư nợ tạm ứng còn lại = dn\_tucl
* Điều khoản thanh toán = ma\_dktt (dùng ở cả bán hàng, mua hàng, yêu cầu báo giá ....)
* Điều khoản giao nhận/ giao hàng = ma\_dkgn (dùng ở mua hàng, bán hàng, kho ...)
* Phương thức thanh toán = pt\_tt (tiền mặt/ chuyển khoản)
* Thanh toán trước ngày = ngay\_tt
* Nội dung chi phí = nd\_cp
* Mã phí = ma\_phi, Tên phí = ten\_phi, Đơn vị tính = dvt
* Đơn giá nguyên tệ = gia\_nt, Số lượng = sl
* Giá bán = gia\_nt/ Giá vốn = gia\_von/ Tiền bán (bán hàng) = tien\_ban/ Tiền vốn (giá vốn hàng bán) = tien\_von
* Thành tiền = tien\_tt, Thành tiền nguyên tệ = tien\_tt\_nt, thành tiền trước thuế = tien\_tt\_tt, thành tiền sau thuế = tien\_tt\_st, Tiền phê duyệt = tien\_pd, Tiền bằng chữ = tien\_bc, Đồng tiền sử dụng: dt\_sd, Tỷ giá: ty\_gia, Tiền nộp = tien\_nop, Thuế suất = thue\_suat
* Số lượng đặt sản xuất = sl\_lsx
* Định mức = **sl\_dm** (bom = bill of material)/ Tỷ lệ hao hụt = **ty\_le\_hh**/
* Số lượng đề xuất = sl\_dnx, Số lượng đề nghị nhập = sl\_dnn, Số lượng thực xuất = sl\_tx, Số lượng mua = sl\_mua
* Bộ phận giao = bp\_giao, Bộ phận nhận = bp\_nhan, Bên bàn giao (trường hợp trong phiếu không biết chính xác bên giao thuộc nhà máy hay là đơn vị bên ngoài) = ben\_giao
* Điều khoản giao nhận/ Bàn giao = ma\_dkbg --> Tại kho|Không qua kho
* Ngày bàn giao = ngay\_giao\_hang
* Ngày kế toán = ngay\_kt
* Số lệnh sản xuất = so\_lsx
* Người giao = nguoi\_giao, Người nhận = nguoi\_nhan
* Người lập = nguoi\_lap
* Người mua hàng = nguoi\_mua\_hang
* Đơn vị tính đề xuất = dvt\_dx (sử dụng trong phiếu xuất kho sử dụng đơn vị tính khác với đơn vị tính mặc định của mã hàng)
* Mã đơn vị tính = ma\_dvt, Tên đơn vị tính = ten\_dvt
* Tỷ lệ quy đổi = tl\_qd (Dùng trong trường hợp quy đổi một giá trị tương đương ra giá trị mặc định, ví dụ: mã vật tư Thép tấm có 2 đơn vị tính kg và tấn ⇒ quy đổi: 1tấn = 1000 kg)
* Số hóa đơn = so\_hoa\_don
* Số hóa đơn nội bộ = so\_hd\_nb
* Ký hiệu hóa đơn = ky\_hieu
* Ngày hóa đơn = ngay\_hoa\_don
* Biển số xe = bien\_so\_xe\`
* Địa bàn tiêu thụ = Khu vực tiêu thụ = "dia\_ban"
* Số lượng xuất = sl\_xuat (dùng trong phiếu điều chuyển kho), Số lượng nhận = sl\_nhan (dùng trong phiếu điều chuyển kho)
* Phát sinh (kế toán)= Phát sinh nợ = ps\_no, phát sinh có = ps\_co
* Tổng phát sinh nợ= tong\_ps\_no, Tổng phát sinh có = tong\_ps\_co
* Phát sinh nợ nguyên tệ = ps\_no\_nt, Phát sinh có nguyên tệ = ps\_co\_nt
* Mã vụ việc = ma\_vv, Tên vụ việc = ten\_vv, Mã vụ việc mẹ = ma\_vv\_me
* Tệp đính kèm = tep\_dk
* Tỷ giá mua vào = tg\_mv, Tỷ giá bán ra = tg\_br
* Mã ngoại tệ = dt\_sd, Tỷ giá = ty\_gia
* Đã thanh toán = da\_thanh\_toan
* Tên viết tắt = ten\_viet\_tat
* Mã phân hệ = ma\_ph, Tên phân hệ = ten\_ph
* Mã thanh toán = ma\_tt
* Nhóm thuế = nhom\_thue

#### **Tên nhóm control liên quan tới Nhân sự** <a href="#nhom_control_lien_quan_toi_nhan_su" id="nhom_control_lien_quan_toi_nhan_su"></a>

* Giới tính = gioi\_tinh
* Ngày sinh = ngay\_sinh
* Địa chỉ hiện tại = dia\_chi\_ht
* Hộ khẩu = ho\_khau
* Tình trạng hôn nhân = tt\_hn
* Dân tộc = dan\_toc
* Tôn giáo = ton\_giao
* Số chứng minh nhân dân = cmnd\_so
* Ngày cấp = cmnd\_ngay
* Nơi cấp = cmnd\_nc
* Mã trợ cấp = ma\_tc
* Tên trợ cấp = ten\_tc
* Số tiền trợ cấp = tien\_tc
* Loại trợ cấp = loai\_tc
* tc\_thang = thángTrợ cấp hàng
* Thông tin liên hệ: Địa chỉ cá nhân = ld\_dccn
* Thông tin liên hệ: Số điện thoại cá nhân = ld\_sdtcn
* Thông tin liên hệ: Email cá nhân = lh\_mcn
* Thông tin liên hệ: Địa chỉ công ty = lh\_dcct
* Thông tin liên hệ: Số điện thoại công ty = lh\_sdtct
* Thông tin liên hệ: Email công ty = lh\_mct
* Thông tin liên hệ: Địa chỉ liên hệ khẩn cấp = lh\_dckc
* Thông tin liên hệ: Số điện thoại liên hệ khẩn cấp = lh\_sdtkc
* Thông tin liên hệ: Mail liên hệ khẩn cấp = lh\_mkc
* Mã dân tộc = ma\_dt
* Tên dân tộc = ten\_dt
* Mã tôn giáo = ma\_tg
* Tên tôn giáo = ten\_tg
* Mã quốc gia = ma\_qg
* Tên quốc gia = ten\_qg
* Mã trình độ học vấn = ma\_hv
* Tên trình độ học vấn = ten\_hv
* Kỳ trả lương = ky\_tra\_luong
* Loại thu nhập = loai\_tn
* Mã thu nhập = ma\_tn
* Tên thu nhập = ten\_tn
* Tính thuế TNCN = thue\_tncn
* Thu nhập bằng tiền = tien\_tn
* Phương pháp tính lương = pp\_tl
* Hình thức thanh toán = ht\_tt
* Phương pháp tính thuế = pp\_tt
* Tên người phụ thuộc = ten\_nguoi\_pt
* Mã thời gian = ma\_thoi\_gian
* Tên thời gian = ten\_thoi\_gian
* Thời gian bắt đầu = tg\_bd
* Thời gian kết thúc = tg\_kt
* Phút quy đổi = phut\_qd; Quy đổi = qd; giờ quy đổi = gio\_qd
* Tổng thời giam làm việc = tong\_tglv
* Ngày trong tuần = ngay\_thu
* Mã ngày nghỉ lễ = ma\_ngay\_nghi; Tên ngày nghỉ lễ = ten\_ngay\_nghi

#### **Tên các control trong bảng** <a href="#cac_control_trong_bang" id="cac_control_trong_bang"></a>

* Tên bảng = "tb"+"xx" (x tịnh tiến từ 1 tới n tùy theo thứ tự khởi tạo của bảng)

#### **Tên control nằm trong bảng = "tbx\_" + "tên control"** <a href="#ten_control_nam_trong_bang_-_-tbx_-_+_-ten_control" id="ten_control_nam_trong_bang_-_-tbx_-_+_-ten_control"></a>

* Số đơn hàng mua = so\_dhm, số Đơn hàng bán = so\_dhb
* Loại chứng từ = loai\_ct (Chứng từ gốc đề kế thừa dữ liệu), Số chứng từ tham chiếu = chứng từ kế thừa = sct\_tc

Danh mục nghiệp vụ = dm\_nv, Mã nghiệp vụ = ma\_nv, Tên nghiệp vụ = ten\_nv

#### Tiêu đề của control <a href="#tieu_de_cua_control" id="tieu_de_cua_control"></a>

Tiêu đều control cần đặt ngắn gọn, viết tắt nhưng vẫn thể hiện được nội dung control

Cụ thể

* Số lượng = SL
* Chất lượng = Clg
* Nhập kho = Nk
* Tồn kho = Tk
* Xuất kho = Xk
* Đại diện = Đ.diện
* Ban giám sát = BG.sát
* Kiểm tra = Ktra
* Kĩ thuật = KT
* Kích thước = K.thước
* Tình trạng = T.trạng = Trạng thái
* Thời gian = Tgian
* Nhiệt độ = N.độ
* Cường độ = C.độ
* Điện áp = Đ.áp
* Hoạt động = H.động
* Hiệu điện thế = Hđ.thế
* Giá trị = G.trị
* Máy biến áp = Mba
* Thông số = T.số
* Trường hợp = T.hợp
* Tổng hợp = TH
* Cài đặt = C.đặt
* Mã chứng từ = Mã CT
* Số chứng từ = Số CT
* Mã sản phẩm = Mã SP
* Mặt phẳng = MP
* Bổ sung = Bsung
* Phế phẩm = PP
* Nhân viên = NV
* Công việc = CV
* Đơn vị tính = Đvt
* Năng suất = NS
* Phân loại = PL
* Nôi dung = ND
* Chỉ số = C.số
* Sản xuất= SX
* Bộ phận = BP
* Nguyên liệu = NL
* Áp suất = AS
* Khu vực = KV

### **Sử dụng control TTSD trong Danh mục** <a href="#cach_dat_ten_cac_control" id="cach_dat_ten_cac_control"></a>

* Việc tạo các Control "ttsd" (trạng thái sử dụng) trong các DOC danh mục là bắt buộc;
* Khi Query và gọi các Item từ Doc danh mục vào sử dụng ở các nơi khác nhau bắt buộc có điều kiện lọc "=1";

### Cấu hình các kiểu view danh sách

* Pin 3 cột thông tin quan trọng ở tất cả các showlist để tiện theo dõi ngay khi tạo doc&#x20;
* Ẩn hết các cột thông tin hệ thống không cần thiết tại showlist ngay khi tạo doc&#x20;

## WORKFLOW

### Xây dựng quy trình

* Luôn phải config Display text cho quy trình: Khi chưa có thông tin số chứng từ/diễn giải của chứng từ đi kèm thì hiển thị “Tên quy trình + Ngày lập”, khi check điều kiện đã có thì chuyển thành hiển thị “Số chứng từ”&#x20;

Ví dụ: Khi mới khởi tạo quy trình phiếu nhu cầu > Tên quy trình là “TẠO PHIẾU NHU CẦU: 2022-12-15"&#x20;

Sau khi bản ghi chứng từ gắn với phiếu nhu cầu được lập thì sẽ ghi nhận được thông tin các biến/trường thông tin trong chứng từ > Tên quy trình phải được cập nhật thành “TẠO PHIẾU NHU CẦU: CVN/MA22120012”&#x20;

* Luôn config tiêu đề task cho các công việc: Khi chưa có thông tin số chứng từ/diễn giải của chứng từ đi kèm thì hiển thị “Tên quy trình + Ngày lập”, khi check điều kiện đã có thì chuyển thành hiển thị “Tên tác vụ + Số chứng từ” (Có thể thay đổi biến số hiển thị theo nhu cầu khách hàng sau)&#x20;
* Luôn config thông tin bổ sung task cho các công việc: Khi chưa có thông tin số chứng từ/diễn giải của chứng từ đi kèm thì hiển thị “Tên quy trình + Ngày lập”, khi check điều kiện đã có thì chuyển thành hiển thị “Diễn giải” (Có thể thay đổi biến số hiển thị theo nhu cầu khách hàng sau)&#x20;
* Các thông tin assignee luôn dùng công thức truy vấn đến orgchart chứ không được gắn người trực tiếp&#x20;

## DATAFLOW

### Báo cáo

#### **Chuẩn hóa Font và Size chữ**&#x20;

* **Level 5( text body) : 12**&#x20;

Là các thông tin nội dung cụ thể trong bảng, cột...hoặc nội dung trục hoành , trục tung trong biểu đồ&#x20;

* **Level 4 (chart legend) : 13**&#x20;

Là các thông tin tên cột của bảng hoặc chú thích của biểu đồ&#x20;

* **Level 3 (chart title) : 15**&#x20;

Là các thông tin tiêu đề biểu đồ, tên của các trường thông tin riêng lẻ&#x20;

* **Level 2 (subtitle) : 24**&#x20;

Là các tiêu đề phụ của doashboard&#x20;

* **Level 1 (title) : 32**&#x20;

Là tiêu đề chính của doashboard&#x20;

Ngoài ra số liệu hiển thị của Card có size là : 26&#x20;

Level 1 (title)&#x20;

Level 2 (subtitle)&#x20;

Level 3 (chart title)&#x20;

Level 4 (chart legend)&#x20;

Level 5 (text body)&#x20;

#### **Cấu hình hiển thị báo cáo**

* Luôn pin 3 cột thông tin quan trong nhất để khi scroll ngang ko bị trôi thông tin&#x20;
* Luôn để báo cáo fit screen&#x20;
* Luôn kiểm tra bố cục của báo cáo để đảm bảo ko có khoảng trống thừa thãi&#x20;
* Các ô lọc để ngang và nhỏ nhất có thể để nhường không gian hiển thị cho các chart thông tin&#x20;
