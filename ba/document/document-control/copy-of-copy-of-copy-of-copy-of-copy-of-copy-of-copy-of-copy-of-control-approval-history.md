# Control Department

## OVERVIEW

Control Department is used **** to the user can select department, role, and user from the org chart, the data outcomes will be saved in form of serial type and separated by “,”.&#x20;

Control Department has type is data input and data type is text.

| Properties                               | Formula                         |
| ---------------------------------------- | ------------------------------- |
| Name <mark style="color:red;">\*</mark>  | In the group include            |
| Title <mark style="color:red;">\*</mark> | Droplist choose orgchart        |
| Width                                    | Droplist choose available level |
| Height                                   | Multiple select link control    |
| Font size                                | Formula active                  |
| Text color                               | Multi-option selector attribute |
| Hidden                                   |                                 |
| Save value                               |                                 |

( <mark style="color:red;">\*</mark> ) For detailed information, click link below.

[document-editor.md](../document-editor.md "mention")

## CONFIG CONTROL DEPARTMENT

### Steps to configure the control department

#### Step 1: Select Orgchart

![Select Org chart](../../.gitbook/assets/d1.png)

Business Analytics selects one org chart from the list of org charts to use as data.

#### Step 2: Select the available level

![Select available level](../../.gitbook/assets/d2.png)

Business Analytics has three options to choose from for displaying org chart data to save one in Department, Role, and User.

#### Step 3: Select control condition

![Select control condition](../../.gitbook/assets/d7.png)

Conditional control displays a droplist of controls that take the value of the user present in the document. The control department displays according to the control condition selected.

At the End user control department screen, only the departments and locations where the user is present under the condited control are displayed.

#### Step 4: Config formula active

![Config formula active](../../.gitbook/assets/d3.png)

Businesses can configure multiple org chart data clusters to display, and writen't or write a formula to activate which cluster to apply.

In case there are more than two org chart data clusters returned for display, it will default to out the first cluster to show.

Business Analytics has a configured option to choose multiple or choose one.

![Choose multiple](<../../.gitbook/assets/d3 (1).png>)

## SHOW CONTROL DEPARTMENT

![Show control department on End User screen](../../.gitbook/assets/d4.png)

![Display as treeview](../../.gitbook/assets/d5.png)

When the End User clicks on the control department, a popup will be displayed and the departments, roles, users. And can choose to display in the form of a treeview.

![Select multiple options](../../.gitbook/assets/d6.png)
