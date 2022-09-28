---
description: 'Common errors when creating document - Writer: Hoanp'
---

# Common errors

#### Name of some control is not valid

Appears when the creator forgot to name the control, or named the control wrong with the rule. Controls that have an invalid name that will appear on the pop up notification and will be outlined in red.

![](<../.gitbook/assets/image (158).png>)

#### Infinite loop

An infinite loop error notification appears when the formulas in the controls are logically incorrect. Usually it's because the data dump is repeated infinitely because the creator wrote the wrong logic in the formula.

**Lỗi chuyển đổi control:**

**\* Lỗi:**

Server Error

ERROR: cannot cast type double precision to date LINE 1: ...y\_kt DATE,ALTER COLUMN ngay\_bd TYPE DATE USING ngay\_bd::DATE ^

**\* Nguyên nhân:** Lỗi xảy ra do việc chuyển đổi control dẫn đên việc thay đổi kiểu dữ liệu gây mất dữ liệu

**\* Giải pháp:** Sử dụng 1 control khác
