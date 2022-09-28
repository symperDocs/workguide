---
description: >-
  To input data, however, users are allowed to select only 1 value from the list
  of values.
---

# Control Select

**How to use control select**: In Formula configuration, enter the list formula for the control, then save it, then just click on the control to automatically appear a list of data, allowing to select 1 value from the list of values

&#x20;**Configure the control in the Attribute bar:**

&#x20;   ****   &#x20;

| Properties:                                                | Formula configuration                            |
| ---------------------------------------------------------- | ------------------------------------------------ |
| Control name<mark style="color:red;">\*</mark>             | Value                                            |
| Control title<mark style="color:red;">\*</mark>            | Visible<mark style="color:red;">\*</mark>        |
| Added information<mark style="color:red;">\*</mark>        | Read-only<mark style="color:red;">\*</mark>      |
| Default value<mark style="color:red;">\*</mark>            | List                                             |
| Width<mark style="color:red;">\*</mark>                    | Link<mark style="color:red;">\*</mark>           |
| Height<mark style="color:red;">\*</mark>                   | Require<mark style="color:red;">\*</mark>        |
| Font size<mark style="color:red;">\*</mark>                | Require change<mark style="color:red;">\*</mark> |
| Text color<mark style="color:red;">\*</mark>               |                                                  |
| Input value<mark style="color:red;">\*</mark>              |                                                  |
| Key cache in table<mark style="color:red;">\*</mark>       |                                                  |
| Quick submit<mark style="color:red;">\*</mark>             |                                                  |
| Allow multiple selection<mark style="color:red;">\*</mark> |                                                  |
| Renew value<mark style="color:red;">\*</mark>              |                                                  |
| Important<mark style="color:red;">\*</mark>                |                                                  |
| Require<mark style="color:red;">\*</mark>                  |                                                  |
| Require change<mark style="color:red;">\*</mark>           |                                                  |
| Exclusive in database<mark style="color:red;">\*</mark>    |                                                  |
| Exclusive in table<mark style="color:red;">\*</mark>       |                                                  |
| Hidden<mark style="color:red;">\*</mark>                   |                                                  |
| Read-only<mark style="color:red;">\*</mark>                |                                                  |
| Save value<mark style="color:red;">\*</mark>               |                                                  |

( <mark style="color:red;">\*</mark> ) For detailed information, click link below.

{% embed url="https://app.gitbook.com/s/-McNyP8y_A8MZOZl5QPQ/c/2iHl77h3duRLjr1segA3/module-document/document-editor" %}
DOCUMENT EDITOR
{% endembed %}



#### Formula value

Use an appropriate expression to set the value for control, the value will be set when submitting the document ( same with default value )

There are two ways to set the value for control:

1. Select directly value

Example:[https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EY4ywBG0WExFuSvf81Dmx58BuqW-8EZMd-RiJ6L36w0v3Q?e=ShJYjj](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EY4ywBG0WExFuSvf81Dmx58BuqW-8EZMd-RiJ6L36w0v3Q?e=ShJYjj)

&#x20; 2\. Select the value from other control in the same document

Example:[https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EbyWSUk3c\_1Ag4HKe250wOIBZtr-8B4jYJzj42r-TInX7g?e=bK4Cup](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EbyWSUk3c\_1Ag4HKe250wOIBZtr-8B4jYJzj42r-TInX7g?e=bK4Cup)

**List Formula:** Use an appropriate expression to list out all the values that could be selected in select, combo box control and input filter box.

Example:[https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ESeAJhwGbblCpSuhpzf82PMB0yqmHVZnmlOp2d3oO5FvpA?e=ks8jtk](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ESeAJhwGbblCpSuhpzf82PMB0yqmHVZnmlOp2d3oO5FvpA?e=ks8jtk)

**Example:**

To select one of the status options of WBS:

```
select * from (values('NEW'),('WIP'), ('DONE'))
```

So when submitting document, when user clicking on the control, a list of 3 states will appear and the user can only choose 1 of all the above options.
