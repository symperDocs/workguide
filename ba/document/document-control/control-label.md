# Control label

**How to use control label :** In Formula configuration, enter the value formula for the control, then save it,the control will display as configured.

**Configure the control in the Attribute bar:**

| Properties:                                                | Formula configuration                     |
| ---------------------------------------------------------- | ----------------------------------------- |
| Control name<mark style="color:red;">\*</mark>             | Link<mark style="color:red;">\*</mark>    |
| Control title<mark style="color:red;">\*</mark>            | Visible<mark style="color:red;">\*</mark> |
| Added information<mark style="color:red;">\*</mark>        | Value                                     |
| Default value<mark style="color:red;">\*</mark>            |                                           |
| Width<mark style="color:red;">\*</mark>                    |                                           |
| Height<mark style="color:red;">\*</mark>                   |                                           |
| Font size<mark style="color:red;">\*</mark>                |                                           |
| Text color<mark style="color:red;">\*</mark>               |                                           |
| Input value<mark style="color:red;">\*</mark>              |                                           |
| Key cache in table<mark style="color:red;">\*</mark>       |                                           |
| Allow multiple selection<mark style="color:red;">\*</mark> |                                           |
| Renew value<mark style="color:red;">\*</mark>              |                                           |
| Important<mark style="color:red;">\*</mark>                |                                           |
| Require<mark style="color:red;">\*</mark>                  |                                           |
| Require change<mark style="color:red;">\*</mark>           |                                           |
| Exclusive in database<mark style="color:red;">\*</mark>    |                                           |
| Exclusive in table<mark style="color:red;">\*</mark>       |                                           |
| Hidden<mark style="color:red;">\*</mark>                   |                                           |
| Allow updates<mark style="color:red;">\*</mark>            |                                           |
| Save value<mark style="color:red;">\*</mark>               |                                           |

( <mark style="color:red;">\*</mark> ) For detailed information, click link below.

{% embed url="https://app.gitbook.com/s/-McNyP8y_A8MZOZl5QPQ/c/2iHl77h3duRLjr1segA3/module-document/document-editor" %}
DOCUMENT EDITOR
{% endembed %}

#### Formula value

Use an appropriate expression to set the value for control, the value will be set when submitting the document ( same with default value )

Example:[https://ywb69zeduvn.sharepoint.com//s/Symper347/EUur3gEbCh1NvHnOwPOdMdYBZWxcJxu0r\_DIv8MGo3h4\_Q?e=GeN6ZY](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EUur3gEbCh1NvHnOwPOdMdYBZWxcJxu0r\_DIv8MGo3h4\_Q?e=GeN6ZY)

### Some tips when using the control Label

It can only allows displaying the data but not editing.

### Example

To automatically generate the module name based on the module code entered:

```
ref(
    SELECT distinct ten_module from dm_symper_module WHERE ma_module = '{ma_module}'
)
```

<figure><img src="../../../.gitbook/assets/image (1) (3).png" alt=""><figcaption></figcaption></figure>
