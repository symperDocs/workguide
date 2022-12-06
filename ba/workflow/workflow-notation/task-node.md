# Task Node

## **Task types**

There is a list of different types of Tasks identified within BPMN to separate the types of inherent behavior that Tasks might represent:

| **ICON**                                                                                                                                                                              | **NAME**               | **DESCRIPTION**                                                                                                         |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------- | ----------------------------------------------------------------------------------------------------------------------- |
| ![](https://lh3.googleusercontent.com/EKLxBbbpQR5TD-TPbhARkLIMfUrSAcPs1X9-JdbNMGGmuMYSSU\_vc51lkwkphmjOLNqOBNbixQFqkPUm9TqAfoWGDgF1-LcI65LGrs1JADZFHSC7SRhRc43--QhdNdLx96esaRH5)      | Task                   | A Task is a rounded corner rectangle that must be drawn with a single thin line.                                        |
| ![](https://lh4.googleusercontent.com/s-8L3lL31KZpNMtyhgsowmmS85Bv\_oCs3Y81IqbL\_KPWHY\_NGU0sCjw8qNMW7YG9A4NYA70utcN0mOz9s0Y1MoHyJUdfbsbVsGakAz4VYlBFT7EYZdp9ARvsAkKDsels49cULdaF)    | User task              | A 'User task' is used to model work that needs to be done by user.                                                      |
| ![](https://lh4.googleusercontent.com/NOioSvzIlaf0Di-vVJgSLAM3-Fcr9vfqm4UJhnvKug4nl1xYqDdwKQibN6mSNwrCMpPnCU1nLH0ZphdhVS4equevzTs8ueskZs4gpVly9PmWkJvxiNwkr4xdOz8HwYj2a8bM510Z)       | <p>Script task<br></p> | A task that is executed on a certain system engine. The engine will check this script/expression to run and do the job. |
| ![](https://lh6.googleusercontent.com/MQ0D7GYL9QaKORNY0sOMNMUGR\_SRdp8NopruX9KhhUEdWkO3URNQ3YMvIeEsKKUT5Baeijfvw0HMj8lfjy0As108a7nqpYCMtTmT38rL\_fWuqTLn3N6Q0a36egM5H\_UOFx9RbDA1)    | Service task           | A task that uses an automated application, or other kinds of service in completing the task.                            |
| ![](https://lh4.googleusercontent.com/qW07oifpdYzyBDFxUDJkugWCCcLLcYLzDyUSsBrEXTh3J76vuPXuenLDSn0x9A0L52lgK6gm6ZK1M6Sui3gmbsHArtL6c2B7rEWVwm2\_Rm5J7ugER\_5DicgykIXCKGHgm2MigDhz)     | Send task              | A task represents sending information, documents.                                                                       |
| ![](https://lh6.googleusercontent.com/X0W2RS96X4Aojyh5VXcSF\_xbXtcwRw6JyOKDAUPYFQj4HDNcnaPjlRUxVtUo4FYCtjIoXI5lgBQpR7OxaqDqMN8-R1KH\_BZ1NUUG\_QUvqu6hqYZV7q4yM5IXyYqmhEJ82JACwfQR)    | Receive task           | <p>A task describes receiving information, documents.<br></p>                                                           |
| ![](https://lh6.googleusercontent.com/vqQte3MwIa7i5Tr43ppX2fRJBhDaSu\_iDsUSVfaGZOpHDGUbrZD8cX7SX0XgRd3jcNdRHDwLJbsDUqLR9NkgM8dY1mIEehOb\_9fOuSd3yeASegHuhCigxa8ebetBdJkwv523HcFu)     | Manual task            | A task that is performed by the user, out of the system.                                                                |
| ![](https://lh6.googleusercontent.com/evT6cDSfmMS9D0zswn4JOy49RDKBA19OA6VZ1bv3koZMFWwyUDdX\_tyVh5ZUMa1PhYlaB8hslbZ137UBSBP37y9ve\_AMKwrjF8ebZ3i8SQl\_CIcIv\_\_P\_SK0r86PbbDlREQTR70T) | Business rule task     | The Business Rule Task represents a task which relies on a certain rule.                                                |
| ![](https://lh3.googleusercontent.com/uFowoDUyL4QGPRYdFJNxQAveBoJ9sGvctpgL8rbgsVk0Sox9cJcrfYAXkCcR2S82N7wSN9HbpduGVHXRS0BQZTt6lv2E\_HOw1K8w6xmgGpskDG5k4mCfSpQYhmz0ZYws6UJk4Zcv)      | Call activity          | Call back a process defined before.                                                                                     |
|                                                                                                                                                                                       | Sub Process            | An embedded subprocess allows to group elements of the process.                                                         |

Sub Process: A sub-process is a compound activity that represents a collection of other tasks and sub-processes. They could both allow you make a logical and more readable diagram for a sequence of activities.

Sub Process have two use cases:\\

***

* **Collapsed** ![](https://lh5.googleusercontent.com/Qlp3yg0ZuIxuUP4DKyr6C\_vFqE7wAFSI5qYw3BH2otoJg5YdbhQUu0kRHsq5VKXn4XLsCRT9cMAwRRHQEk0DKcRC5HVFlhoCKzCoLf1NoxLtqEfinCDDwfd1RQIkzDKAQ9DAgVZC)**:** The details are not visible in the process diagram, you may press this task, then you will see the details on another page. It makes the visualization of the business process a lot easier.
* **Expanded** ![](https://lh5.googleusercontent.com/HP2Pc0EYra3CG-R3axmx8zV8r7w4ec53ZcoZrNNpo57pLIbkKG4QmIObJC9rBsRc3DdOIWZEEirnuyD6WjNWtom1X-Ltt2FcQrlBxOKgpLfOf5EBRuj6gYtfUJruNMuQ4tc3VtKQ)**:** All its details are shown within its limits instead of a new page. In my opinion, compared to Collapsed Sub-Process, it is more intuitive without executing any hyperlinks. The part of Task on the following picture is an example of Expanded Sub-Process.

## **Activity Markers**

| ![](https://lh4.googleusercontent.com/Djv12UFgje6Vg2RWatYC1CpapWuSTFoUXD-Llq7LBhoIBqLBnJK-iy5x9msDwGXxSiHH-gPh12Gme4sHITtw40hKbPH7N1oRnpH4R7R6VGYst471joZ2dkwuteXNq8YBetoRon9T)     | Parallel Multi-Instance   | The action is repeated many times, but it needs different data sets and do at the same time |
| ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------- | ------------------------------------------------------------------------------------------- |
| ![](https://lh6.googleusercontent.com/JzKczZ0fOWCUrcCK\_TWshv\_R\_hEzIROUaez69yN6KXyTnycbwlxMVu3s1N65TvClfL3mYPWYzBdYbvOx0D4yA3MdpoHMk4zr-l4M6DYR9xVXbqA57\_65xit0L9f8tlvPzp6UPxAS) | Sequential Multi-Instance | The action is repeated many times, but it needs different data sets and do it sequence      |
| ![](https://lh5.googleusercontent.com/GSroVoi6IN8cZEjVTXxFQTVUsI7zTyh07pRqgtKJIRHvMTs8ZWn2s88afNe1UNKWszbnxT-UIXStQA6L54rtGh8D\_99nkdmL5ljnCTRnm17P7CXXg1c1ooiSasxWhWcWmtsT\_GYA)   | Loop                      | Repeated in sequence.                                                                       |
| ![](https://lh4.googleusercontent.com/GiF0de9HA-h9Dkfmd-o4nCdNNPAetdGdSkbwOZDfviZF21abXmS18VVgjyc3vVi-ebYxSeZgf11NPxl9gzewjDUknFBCYa7YHNGoLJIWVbkmxGhFMcH7QnJKvMzlSO\_M3z0W0SxB)    | Ad hoc                    | Represents special tasks that have a specific purpose                                       |
| ![](https://lh5.googleusercontent.com/WRYdRFGegHn57oIEZHB8EK3T3vkh-JOHswn6nhYva07z-Is9QotKyxSpZ2wpWlwfZE3Q-xHbYcOWFF245HEoykKYS9N9NkIUHyV3xh108qRXgd--cCg3vP-cCqMtbx0cCizNbrqk)     | Compensation              | Only happens after a specific task                                                          |

### Multi instance

Which is an action that repeats many times but needs different data sets

* **Parallel**: The action is repeated many times, but it needs different data sets and do at the same time

<figure><img src="../../../.gitbook/assets/image (9) (1).png" alt=""><figcaption><p>Activity Multi-Instance marker for parallel instances</p></figcaption></figure>

* **Sequential:** The action is repeated many times, but it needs different data sets and do it sequence

<figure><img src="../../../.gitbook/assets/image (8) (4).png" alt=""><figcaption><p>Activity Multi-Instance marker for sequential instances</p></figcaption></figure>

**Example:**

![](https://lh6.googleusercontent.com/lzBL9E1wZUAdbFP3Kxa5W4LT7TJ43qibB9sxbYMsY1l-TnXCg7xdTjhtE3UmlMU1QQEpF1yL1yCdEpH-u3ABXM5mrVPOF53jy0t7XjXZ4wQ8wxYSScy9pt52J7UJPXf9OGKj9cWp)

**+ Parallel:** In the editing draft step, you have to edit it many times, you can ask a colleague to do the same. Each editor will have a different data set at the same time

**+ Sequential:** if you use Sequential, then when person A finishes editing, he will take the draft to send to B for editing, person A will fix it, then it will be person B's turn. Continue until the end\\

***

### **Loop**

Similar to Multi instance but without using different data sets. Repeat the edit draft step until it is accepted and then move on to the next step (approval)

<figure><img src="../../../.gitbook/assets/image (3) (3) (2) (1).png" alt=""><figcaption><p>A Task object with a Standard Loop Marker</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (13) (4) (1) (1).png" alt=""><figcaption><p>A Sub-Process object with a Standard Loop Marker</p></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (11) (2).png" alt=""><figcaption><p>Loop task</p></figcaption></figure>

### **Ad hoc**

Represents special tasks that have a specific purpose, usually located in Sub Process, this marker only show the meaning, does not have special features\\

Use the ad-hoc sub-process to mark a segment in which the contained activities (tasks or sub-processes) can be:

* Executed in any order,
* Executed several times, or
*   Skipped\
    \*\*\*\*\\

    ***

![](https://lh6.googleusercontent.com/Za7yufUcGtoh5qDEmHx8-Q0sJwfPMdvvKkZ5\_sTsoUCV1RNhwjpu9qHgzQZ7BlcCZnsEe1qzTXT1zkPtXZPtzmTBN4BSpT0CmyXg2HnjGctKV6NvIMeEzq4Jr8iRyrcC8hOKapQv)

### **Compensation**

Only happens after a specific task.

The Compensation Marker may be used in combination with the loop marker or the multi-instance marker. The Compensation task allows rolling back to the original state if the processing operation fails.

<figure><img src="../../../.gitbook/assets/image (6) (4).png" alt=""><figcaption><p>The 'Pay editor' task turns up only when it has the 'Edit draft' task before</p></figcaption></figure>

## **User manual**

To use these tasks, drag this icon and drop it outside the menu bar

![](https://lh4.googleusercontent.com/EwPVThoP\_PmMg3ClS2ICgCmQ-kj99n7q8SrwTcDGtWSajWiD44gOVeCBHwRVTXtkYWArZH\_UflIGTmZhxwySuvAWDwDQ5sa0FeBaqx2KrwIlh2LIOiktJIMZsHxlKRn5kUgkvcHC)

Click to this icon to change task type

![](https://lh3.googleusercontent.com/Fn7mV9LJJDv4q4RPU43di2staBwMfz3rBBhij\_AtUlh9y6mgzcERIBdLpA73-vqeRwNIGoa4I9vr7t5FjYmQlY-tfdz-47A5UlYV8C5ZUzD0D8wonLPj-dS3TATn5sLoMF4j0COI)

A popup will be display list of tasks type and activity makers

![](https://lh5.googleusercontent.com/VAESFNw6m\_6fDqCgry5yGb6vNOxUn30geUGap8VJvOk3UxgfTg-glZTbl0Z2QQEnLYOMotd2W3OH6gf0aJb4\_UvpypeVtXZM64SZ\_8zZvVYSGKjen4-DZxiGItIdgqv4s\_hGoYmc)

**Config:** For manipulating data in the Symper platform, SYQL, JUEL can be used. For more details and guides, access link here:

User task are used when they need someone to execute, with or without conditions.

User task has 6 attributes, other nodes may have fewer attributes\\

***

![](https://lh5.googleusercontent.com/ZWyLHEwGuHWmSYkDE9jcc2P\_1ci2s3vdQSd5U9wH7vL3CsFG9p7TqBGXhj9NxWxAr7F83mAVTtoF8uL0iq4njD6kQ-UP4kQDklkVkdd4\_JGeC7jWpV6zcPNHfZlTfj\_-7mo4KJzT)

### **General**

![](https://lh3.googleusercontent.com/0kSNrgx40zYJ1\_foMd8IWRQmXz40b0Zlk87gFPBAyq4X2I945kWd4Dy2aWvWg98wyt8Eaqas0YetsIUV7rJLOsIif5zjUE99B1Q22mU04wavUhSJEs8KqMJ83W9ies83rGIF-zoO)

* **ID:** is the id of the node, cannot coincide with other ids in a process, can use a formula to query the node by id.
* **Name:** The display name of node, can coincide

![](https://lh3.googleusercontent.com/SVirHXK\_azE42ONo-x0Do0sztvGNKCbeKEKykikLp08QgoxN6kSJ-eUoW2TawPhINSiWnXxp5iH11g73fIXj1dThZj\_uF-ciCiRuGu9uyLjmeXadBHarM-FamLxIAOLjvg7jqJ1r)

*   **Description:** Describe the meaning of node\\

    ***

### **Task action**

There are 4 actions selectable in this task _(Submit, Approval, Update document, Undefined action)_

#### \*\* **\_**Submit\*\*\_

**Form reference:** is used to enter data and perform actions

**Default values:** selected fields in doc to insert default value on initialization with formula

![](https://lh3.googleusercontent.com/HV6vNBcwDQIizVne-t1cnBKgqBYvLizXCaw0F9NopyAPSwt7XcNDqiseTU7rrYSC3z6CytYN6BWKnZ6OOgB6pxHvAlorlrZ2lu15fOKY4HTTG\_AjIe9ubXgaAelnnBew8BhRlXml)

#### \*\* **\_**Approval\*\*\_

**Outcomes:** Can configure actions to execute (Approval, update, reject,.....)

**Approval for element:** Select the task to perform this action

**Editable controls on approval:** fields that are allowed to be edited are for the person assigned on this task\\

***

![](https://lh4.googleusercontent.com/29RnCwhcP5tky0w4Ucn5bX5Zt-59PXOTlFj2oOeHlwfC59daIZ\_5edI6\_9ghzW9B3hh5JILWwDjR7aNcEeqwXWLwEmUI0nZgwy0-FFnWQJjzKr4IwFV5kTbPaQCHAoZznEnl2Oty)

#### _**Update document**_

**Update for element:** choose a specified document to update

![](https://lh5.googleusercontent.com/XzZzq5hs6\_vmMm7xllsk8w3jIVSdjLtcSb7HO3V4Y27N3\_OY4e1TWGwm\_E-0NFQOTgaQ8iJ7Qr6sGr5777avhNihN3Bw7931EpEJk6vn\_QHLMYVclWjjFK5oo3tmbvxiPhvTjwwV)

#### _**Undefined**_

![](https://lh5.googleusercontent.com/L3iB2UXSomhLhZUaahUKf64bwVDDklwuPyr-74icuKKLo7XVN\_2F9AYR6dMKHftiogvWZuzh0AJnttmPmM4HPDi-MEs2SJV9V7ZTXdypntU2AW8MpiSlF9AFQF8ONKknfeKGDHSK)

**Update for element:** choose document to update

### **Assignment**

Task node will automatically update as the user task if the assigned person has been assigned (can be assigned by formula or assigned directly from org chart)

![](https://lh4.googleusercontent.com/9wi0APXvRNbvzqwqbz8\_dizFr0vFXgiv8tOZ6HcVEIksOtkvMQYIAwBJLetbzMc3eMa4bKJcHQGM7lr3MT1sytQOr5sz524Y6A64RYFr9gqBQXNuCgwceqQKp5ZLHLWS-Rqj6GTS)

**Assignment with formula and conditions**

![](https://lh4.googleusercontent.com/6YkziOERg8Oq9QZeF7cXT89pEVQmWDA7zgr3CgsCZ6fVjl1qw90ffeAPhtM7naoAPdax70WGTA1rUOQQHwJQ9EpBGBq55v8MQ\_6wwQL7qhqgoGO6x5c13\_69nYH1lkMUT\_Y\_MyGo)

### **Formula**

Add description for task when receiving notification or when receiving task in myitem

![](https://lh6.googleusercontent.com/ETVnl4mcU87r1qJTaL1GgVXMjH6oSlbh1rh-Eq\_Vr7DnPu7DjgLV\_DzLImR1ZonaYhDMZ8zceQXQJ4vyvefEW\_N\_aSDdwPGUji7Ghl7JAthpF6f3xuW-1VRaRcQY3K\_xRN0Ai96A)

### **Detail**

* **Due date:** time to complete the task
* **Priority:** task priority
* **Category:** Description of task type

![](https://lh5.googleusercontent.com/KWC4aDuoq1keMfM8l8k9Q2k7aO0Fo9C-aTq2iUv1\_Z0YSnJ1bwziVIUGzk1rW\_aPxnBTN5NDqDMBtTgr1u3BZnt4gQ6\_QCCiEGorAIpN11V3YRk9jI69piwh4IKB-uh312f4G-45)

### **Multi instance**

![](https://lh5.googleusercontent.com/KSLVeOf3HD68xIGUxf3ZZ0xRYH9Uz93osQULOFVwThjl\_lBSABaLyudYOCD0LWsCpwnuW1MwD6aUxuMut6VGev6qBYldY2QzWICmxCeEohEXoa0Kmw\_6WvUOi-hD5JuufmH7LF1o)

**Service Task:** Can choose “Script”, “Notification” or "Set variables" in Service task type.

\- If choose “Script”, you will have to need to fill the blank below.

![](https://lh6.googleusercontent.com/eXaHApTtmxJDS7rLA\_WI7UrmOPc6NDWrndeFkiKq5swEe\_Q444jBvncTeO6hQHzrZSClf2rSURN57\_Wx99sefXj0Y4Ab-KdgHVCiCN5Dt-ce7Dyvtsg-u8BrLEEPnBcMXOAntvcm)

This formula use for update status of document with condition specified by user (or any formula for auto complete task).

\- If choose “Notification”, need to fill at Receiver: `${tech_lead_executor_id}`

and Title: `${qa_test_executor_fullname}` Xác nhận hoàn thành bug `${rp_id_bug}`.

This formula sends a notification to a designated person with content in the Title field.

![](https://lh3.googleusercontent.com/QxtEweoBIophWQMd3V5OJiQC8QPaKOQhINR0Ion15KdvyNYT3SShJ2VAnu6xL5Zgy3m3MGfDbu\_iOMeHliPTccS4-EDEUdBCdbFpHjvhyw8tZWCf1do-Ow8\_hVOGPlEtZYmvVDIl)

\- If choose “Set variables”, you will have to need to fill the table below.

<figure><img src="../../../.gitbook/assets/image (2) (1) (1).png" alt=""><figcaption></figcaption></figure>

In the "Name" column, fill in the variable name you want to reset or change the value. For example, if you want to reset the variables "pnh\_sct" and "pgh\_sct" to null value, set the "Value" column blank. Do not fill "null" in the "Value" column or those variables will change into "null" in text. Besides, remember to use the “Set variables” function of Service Task before node User Task in order to take action to activate the changing of variables. If not, those variables will not be set to the value you want.

**Script task:** similar with the Service task

```sql
ref( 
    INSERT INTO symper_wbs (id_bug, tmg_assignee) 
    VALUES ('{id_bug}', '{tmg_assignee}') 
    ) 
```

This formula is used to insert values into specified data fields\
\*\*\*\*\\

***

![](https://lh6.googleusercontent.com/KUDYCOi9AqA2o8juTod\_DPVP06JUNSRfoQTWuY-JMzSQrq4ZIdzbQXdti\_Wl3G4JhDATCAioh-yohWLi2W-OiYfj8XypsLt6Rkph4denfxbHkk7Ip2yViRL8UusS19LyCC4LZLsA)

**Call activity:** Select the process to call in “Call element” and create name in “Name”

![](https://lh5.googleusercontent.com/evXoKG\_i2EnDqZG9geKn\_1VlND3wgje-4lfoNmyvRQN7x3jlWMsUh2erW21QGswjbeNfM-6CzFdRvSNfomwuY-5ry\_Yh9NJuL7j\_RJFMwGIXsNldJh05H6Yppv67UbYe6fFlJWw4)
