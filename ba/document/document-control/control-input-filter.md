# Control Input filter

## OVERVIEW

Control Input filter is used \*\*\*\* multiple selections from a list, the data outcomes will be saved in form of serial type and separated by “,”.

Note: users need to enter a list formula to use control.

| Properties:                                                | Formula configuration                            |
| ---------------------------------------------------------- | ------------------------------------------------ |
| Control name<mark style="color:red;">\*</mark>             | Value                                            |
| Control title<mark style="color:red;">\*</mark>            | Visible<mark style="color:red;">\*</mark>        |
| Added information<mark style="color:red;">\*</mark>        | Read-only<mark style="color:red;">\*</mark>      |
| Default value<mark style="color:red;">\*</mark>            | Visible<mark style="color:red;">\*</mark>        |
| Width<mark style="color:red;">\*</mark>                    | Require<mark style="color:red;">\*</mark>        |
| Height<mark style="color:red;">\*</mark>                   | Require change<mark style="color:red;">\*</mark> |
| Font size<mark style="color:red;">\*</mark>                | Validate<mark style="color:red;">\*</mark>       |
| Text color<mark style="color:red;">\*</mark>               | Link<mark style="color:red;">\*</mark>           |
| Input value<mark style="color:red;">\*</mark>              | List                                             |
| Key cache in table<mark style="color:red;">\*</mark>       |                                                  |
| Renew value<mark style="color:red;">\*</mark>              |                                                  |
| Allow multiple selection<mark style="color:red;">\*</mark> |                                                  |

( <mark style="color:red;">\*</mark> ) For detailed information, click link below.

{% content-ref url="../document-editor.md" %}
[document-editor.md](../document-editor.md)
{% endcontent-ref %}

#### Value Formula:

Use an appropriate expression to set the value for control, the value will be set when submitting the document ( same with default value ).

There are three ways to set the value for control:

1. Select directly value

Example: [https://ywb69zeduvn.sharepoint.com//s/Symper347/EXScc-z3MRRHngRd\_jn4EI0BCtRo-P2HcK6-WPo1-PG8rg?e=89XOtk](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EXScc-z3MRRHngRd\_jn4EI0BCtRo-P2HcK6-WPo1-PG8rg?e=89XOtk)

2\. Select the value from other control in the same document

Example: [https://ywb69zeduvn.sharepoint.com//s/Symper347/EdOxKb7yDsVHjatxLkkCTfIB0ZSRpB7a-gokkxYXvukKkA?e=tOHdBH](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EdOxKb7yDsVHjatxLkkCTfIB0ZSRpB7a-gokkxYXvukKkA?e=tOHdBH)

3\. Select the value from other control in the other document.

Example: [https://ywb69zeduvn.sharepoint.com//s/Symper347/ERfrmNGPWJBJv\_W4etAgqCMBQk-cWX2vyUpPshIaa37dOA?e=5pbes0](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ERfrmNGPWJBJv\_W4etAgqCMBQk-cWX2vyUpPshIaa37dOA?e=5pbes0)

**List formula:** use an appropriate expression to list out all the values that could be selected in select, combo box control, and input filter box.

Example: [https://ywb69zeduvn.sharepoint.com//s/Symper347/EQGWPNxEJkBKlr8ZGHoJKsgBV1Ef04yvFlssF\_Nyq8rzOA?e=0pyOVX](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EQGWPNxEJkBKlr8ZGHoJKsgBV1Ef04yvFlssF\_Nyq8rzOA?e=0pyOVX)

**Example:**

To query a list of level 3 products (dsp\_c3) from document Đơn đặt hàng provided that dspc3 is the same as the search term and the planned production period (ky\_kh) is equal to the planning period the user selected above in the document.

<figure><img src="../../../.gitbook/assets/image (104) (1).png" alt=""><figcaption></figcaption></figure>
