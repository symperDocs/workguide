---
description: >-
  To input data and display date. It offers a convenient way to select a date
  when submitting documents. (Format for displaying date in Symper platform:
  dd/mm/yyyy, format in database:  yyyy/mm/dd)
---

# Control Date

**How to use control date:**

&#x20; **-** Manual input: Enter the configured time format correctly, if it is not correct, an error will be reported

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/Eb1OZrDSH75BntVO9crDnUcBghwMr0X7Ko4BVAA5-taqdA?e=ycogpz](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/Eb1OZrDSH75BntVO9crDnUcBghwMr0X7Ko4BVAA5-taqdA?e=ycogpz)

&#x20;\- Fast input feature:&#x20;

\+ Enter 1 character:  1-> 01/10/2021  (month and year of the present)

Note: must enter positive number

\+ Enter 2 character: 16 ->16/10/2021 (month and year of the present)

Note: do not enter a positive number beyond the date range of the current month

&#x20;( 32 -> report an error)

&#x20;Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EbMYaodry7ZPmgW61IxVTNIBUX8TrLrN27W6HsuUZzrXJQ?e=acZQc8](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EbMYaodry7ZPmgW61IxVTNIBUX8TrLrN27W6HsuUZzrXJQ?e=acZQc8)

&#x20; \+ Enter 1 character concatenated with 1 character with a separator (-, /):

enter 1-1 or 1/1 -> 01-01-2021

&#x20; \+ Enter 2 character concatenated with 2 character with a separator (-, /):

enter 10-10 or 10/10 -> 10-10-2021&#x20;

Note: do not enter more than the date range of the month in the first 2 characters that are not in the month range of the following 2 characters (February does not have 30 days), the following 2 characters do not exceed 12 (enter 30-13 or 30/13 -> Invalid data error)

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EePJ7Umr90tPvht-QxHRdA8BNlUDdf9eYE5oeBhzfq0lEw?e=NE9672](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EePJ7Umr90tPvht-QxHRdA8BNlUDdf9eYE5oeBhzfq0lEw?e=NE9672)

&#x20; \- Select date in calendar field:&#x20;

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EYBTfNS9M1BItjXROosuHmcBbWYa0Y3soiC\_XYatHXX9Xw?e=fdkL7q](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EYBTfNS9M1BItjXROosuHmcBbWYa0Y3soiC\_XYatHXX9Xw?e=fdkL7q)

| Properties:                                                | Formula configuration                            |
| ---------------------------------------------------------- | ------------------------------------------------ |
| Control name<mark style="color:red;">\*</mark>             | Value                                            |
| Control title<mark style="color:red;">\*</mark>            | Hidden<mark style="color:red;">\*</mark>         |
| Default value<mark style="color:red;">\*</mark>            | Read-only<mark style="color:red;">`*`</mark>     |
| Width<mark style="color:red;">\*</mark>                    | Require<mark style="color:red;">\*</mark>        |
| Height<mark style="color:red;">\*</mark>                   | Require change<mark style="color:red;">\*</mark> |
| Font size<mark style="color:red;">\*</mark>                | Start day                                        |
| Text color<mark style="color:red;">\*</mark>               | End date                                         |
| Date format                                                |                                                  |
| Key cache in table<mark style="color:red;">\*</mark>       |                                                  |
| Allow multiple selection<mark style="color:red;">\*</mark> |                                                  |
| Renew value<mark style="color:red;">\*</mark>              |                                                  |
| Important<mark style="color:red;">\*</mark>                |                                                  |
| Require<mark style="color:red;">\*</mark>                  |                                                  |
| Require change<mark style="color:red;">\*</mark>           |                                                  |
| Exclusive in database<mark style="color:red;">\*</mark>    |                                                  |
| Exclusive in table<mark style="color:red;">\*</mark>       |                                                  |
| Hidden<mark style="color:red;">\*</mark>                   |                                                  |
| Read-only<mark style="color:red;">`*`</mark>               |                                                  |
| Save value<mark style="color:red;">`*`</mark>              |                                                  |

( <mark style="color:red;">\*</mark> ) For detailed information, click link below.

**Example:**

To automatically get the current date in 7th time zone:

![](<../../.gitbook/assets/image (30).png>)

{% embed url="https://app.gitbook.com/s/-McNyP8y_A8MZOZl5QPQ/c/2iHl77h3duRLjr1segA3/module-document/document-editor" %}
DOCUMENT EDITOR
{% endembed %}



#### Formula value

Use an appropriate expression to set the value for control, the value will be set when submitting the document ( same with default value )

There are three ways to set the value for control:

1. Select directly value

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EXAzfDueSyFKvZIc2jE\_zZ4BAGs5hJzVdN0zbDNBzlFxMw?e=s3x7Jf](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EXAzfDueSyFKvZIc2jE\_zZ4BAGs5hJzVdN0zbDNBzlFxMw?e=s3x7Jf)

&#x20; 2\. Select the value from other control in the same document

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EYFlESn2zjpDmK7KtSnIsnUBD8SjaeK9Ve7U-3inhEF1PA?e=9NsHhZ](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EYFlESn2zjpDmK7KtSnIsnUBD8SjaeK9Ve7U-3inhEF1PA?e=9NsHhZ)

&#x20; 3.Select the value from other control in the other document.

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EcIBFtB7MvhJjJ8-F6Wk63kB2tCOj5p-Pk3f0w6X6MnIBA?e=ruf63K](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/EcIBFtB7MvhJjJ8-F6Wk63kB2tCOj5p-Pk3f0w6X6MnIBA?e=ruf63K)

**Date format:** Enter the format manually or select a format from the list

Example: [https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ETYM2sty56xKkQm590oKGKYBtLD6asrUQ3VHzYStrGbPdA?e=RJ3dXI](https://ywb69zeduvn.sharepoint.com/:v:/s/Symper347/ETYM2sty56xKkQm590oKGKYBtLD6asrUQ3VHzYStrGbPdA?e=RJ3dXI)
