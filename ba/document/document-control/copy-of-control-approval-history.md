# Control Table

## OVERVIEW

Control table is used to input and display data in the form of table. Control table may consist of all other controls but itself - control table. Only 1 control could be in a cell of a table.

| Properties:                                        | Formula configuration                       |
| -------------------------------------------------- | ------------------------------------------- |
| Control name<mark style="color:red;">\*</mark>     | Value<mark style="color:red;">\*</mark>     |
| Control title<mark style="color:red;">\*</mark>    | Visible<mark style="color:red;">\*</mark>   |
| More information<mark style="color:red;">\*</mark> | Read-only<mark style="color:red;">\*</mark> |
| Display form                                       | Allows deleting existing lines at update    |
| Font size<mark style="color:red;">\*</mark>        |                                             |
| Text color<mark style="color:red;">\*</mark>       |                                             |
| Select identifier field                            |                                             |
| Allows multiple selection                          |                                             |
| Renew value<mark style="color:red;">\*</mark>      |                                             |
| Visible<mark style="color:red;">\*</mark>          |                                             |
| Wrap text                                          |                                             |
| Read-only<mark style="color:red;">\*</mark>        |                                             |
| Allow adding lines                                 |                                             |

( \* ) For detailed information, click link below.

{% embed url="https://app.gitbook.com/s/-McNyP8y_A8MZOZl5QPQ/c/3H9KTihsXr3Cq7tNLHd1/module-document/document-control/control-title" %}
DOCUMENT EDITOR
{% endembed %}

#### Display form

Flat: A flat table is very convenient for entering data.

Pivot: A pivot table is used to summarise, sort, reorganize, group, count, total or average data stored in a table. It allows users to transform columns into rows and rows into columns. It allows grouping by any field (column), and using advanced calculations on them.

Group: A group table is used to group lines, total data on each group.

[https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EfzI7-\_5C-1ImmDmZR4EZKkB0w4nPwkmBNh9viyU3if0Tw?e=RTmJeT](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EfzI7-\_5C-1ImmDmZR4EZKkB0w4nPwkmBNh9viyU3if0Tw?e=RTmJeT)

#### Wrap text

[https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EY8t0WixiV5AnxPlAZxqT0QB4WQU2iAZRS2WQNDDSIbwOw?e=1crfPQ](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EY8t0WixiV5AnxPlAZxqT0QB4WQU2iAZRS2WQNDDSIbwOw?e=1crfPQ)

#### Allow adding lines

[https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ETorjkDnCGtIvzLin8lRgcgBWOACFMZ0DUtoAng3BdyAvw?e=xZvJta](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ETorjkDnCGtIvzLin8lRgcgBWOACFMZ0DUtoAng3BdyAvw?e=xZvJta)

#### Allows deleting existing lines at update

### Some tips when using the control Table

{% embed url="https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EcCwFzndZLpEmHVo9tCZfbEB_11oL7umqZviD7Rg8HSD5g?e=n9LrFU" %}

**Example**

To query mutiple controls from other document in server:

```
ref(
    SELECT distinct
        id_bug as tb4_id_bug, 
        tmg_name as tb4_description,
        tmg_due_date as tb4_due_date, 
        tmg_assignee as tb4_dev
    from
        rd_issue_tracking
    where
        id_bug in {id_issue_kethua}
)
```
