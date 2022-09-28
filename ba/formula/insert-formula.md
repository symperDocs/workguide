# Insert Formula

## INSERT

Insert command is used to insert new records in a table

This query formula can be divided into 2 types:

\+ Insert into data out of table

```sql
INSERT( INSERT into document_symper_xin_nghi (nguoi_nghi, phong_ban, document_object_uuid)
VALUES ('Minh','BA', uuid_generate_v4())
RETURNING document_object_uuid as object_id, 'symper_xin_nghi' as table_name))
```

NOTE:

* Must have prefix 'document' before the document name
* Must have row 'RETURNING .....'
*   Syntax 'uuid\_generate\_v4()' is fixed

    <figure><img src="../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

\+ Insert into data in table

```sql
INSERT (INSERT INTO document_child_lich_lam_viec_tb1 (tb1_day, document_object_uuid, document_object_parent_uuid)
VALUES ('Monday', uuid_generate_v4(), '610752a6-10f9-552f-e767-08f27b120ea0'))
```

NOTE:

* Must have prefix 'document\_child' before the document name
* Must have suffix '\_tbn' (n =1,2,3,4, ....) after the document name
* Syntax 'uuid\_generate\_v4()' is fixed
*   Don't have row 'RETURNING ....' like upon syntax

    <figure><img src="../../.gitbook/assets/image (10) (2).png" alt=""><figcaption></figcaption></figure>

## Auto returing document number (makePrimaryKey)

To auto returning uniue document number for each document instance you insert, you can use `makePrimaryKey` in Insert formula to do this.

For instance:

```
ref(INSERT(INSERT INTO document_symper_wbs ( 
ngay_start , tmg_status ,wbs_id, document_object_uuid )
VALUES (
'{rp_ngay}', 'NEW' , 
makePrimaryKey(symper_wbs, wbs_id,{"ngay_start":"{rp_ngay}"}) ,uuid_generate_v4()
)
RETURNING document_object_uuid as object_id , 'symper_wbs' as table_name
)
)
```

`symper_wbs` is the name of the document you want to insert

`wbs_id` is the control of document symper\_wbs you want to return document number

`ngay_start` is another control in `wbs_id`, data of control `ngay_start` will be put into control `wbs_id` and then based on that to create document number. If the control you want to return document number has more controls in its formula, you need to list down all of the controls in `makePrimaryKey` formula.

`rp_ngay` is the control you get values from `rd_issue_tracking`
