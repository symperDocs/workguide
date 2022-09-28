---
description: 'Writer: Hoanp'
---

# Kaban

## DEFINITION

* Kanban boards: are tools for visualizing work. The Kanban board consists of columns corresponding to the status of the task and cards representing the tasks. Each task when in any state is placed in the corresponding column
* Kanban card: is an image representing a work item

## IBENEFITS OF KANBAN

* Flexible planning: A Kanban team will focus only on the work in progress. Product owners are free to reorder the backlog without disrupting the team because any changes outside of the current work items don't affect the team. As long as the product owner keeps the most important work items of the backlog intact.
* Shortened cycle times: Shared skills mean that team members can take on heterogeneous work, further optimizing cycle times.
* Improvement: measure efficiency by tracking quality, lead time, and more. From there, there are analyzes and tests to change the system to increase the effectiveness of the group.

## HOW TO ACCESS TO KANBAN ON THE SYSTEM

**Step 1**. Log in to the system

**Step 2.** Go to “**My Applications**”, select the app that contains the application you want to see its kanban form (provided that the application already has a kanban)

**Step 3.** Click on the voucher you want to see the kanban, select “**Kanban**”

<figure><img src="../../.gitbook/assets/image (38) (2) (2) (2).png" alt=""><figcaption></figcaption></figure>

## HOW TO CREATE 1 KANBAN

To create 1 kanban for a document that does not have a kanban (remember that each document will have exactly 1 kanban), we follow the steps below in turn:

**Step 1**. Log in to the system, select “**Manage view**”, select “**Kanban**”

**Step 2**. After the screen shows the list of kanbans, click “**Add**”

<figure><img src="../../.gitbook/assets/image (34) (1) (1) (1) (1) (2).png" alt=""><figcaption></figcaption></figure>

**Step 3**. At Step 1 in settings, enter name, description and select document to build kanban

<figure><img src="../../.gitbook/assets/image (3) (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

**Step 4**. At Step 2, select the control in the document whose value will be the columns in the Kanban. Enter the name and value in the selected control for each column. Columns can be added/removed if needed, but each Kanban requires a minimum of 2 columns.

<figure><img src="../../.gitbook/assets/image (40) (1) (1) (1) (2) (1).png" alt=""><figcaption></figcaption></figure>

**Step 5.** In Step 3 of Create kanban, drag and drop columns and arrows between them in the canvas showing the direction that allows dragging cards back and forth between them. It is required to name the stateflow to serve the Access Control part. If you do not set anything here, it will default to all cards being dragged freely between all columns.

![](../.gitbook/assets/image%20\(61\).png)

**Step 6.** Step 4 of Create kanban allows you to select the data control corresponding to each information field of the card and create a condition format for the card. Each format must be named differently.

![](../.gitbook/assets/image%20\(238\).png)

**Step 7**. Click “**Save**” to finish creating new Kanban.

## LOGIC OF THE KANBAN IN SYMPER

### KANBAN WBS

Kanban WBS serves to track and transfer work status of each person.

![](../.gitbook/assets/image%20\(247\).png)

Drag and drop logic:

* NEW to WIP: Everyone has drag and drop permission. Perform drag and drop as each person's work is being in process.
* NEW to DONE or WIP to DONE: Everyone has the right to drag and drop. This shows that the person's work has been completed.
* NEW to REVIEW: No one has drag and drop permission, but WBS will automatically change the status to "REVIEW" every time someone updates the WBS record and edits the **Plan End Date** information. When the task is in the REVIEW column, it will have to be reviewed and approved by the manager/mentor by dragging it to the TO DO column
* REVIEW to TO DO: Only those given the "Admin WBS" role can drag and drop. Dragging the card from REVIEW to TO DO shows the admin's approval for changing the due date of that task.
* TO DO to NEW/ TO DO to WIP/ TO DO to DONE: Everyone has the right to drag and drop. Drag and drop in case that task has a change of due date and admin approved it, and assignee drag and drop them in turn in In-Progress/Completed cases.

Update data:

* Each card dragged to the DONE column will be automatically updated with the **Actual End Date** with the current date (today).
* Control **Actual Time** does not generate data by itself, requiring input before dragging and dropping.
* Each card when dragged to the DONE column will have the total execution time of the child- tasks below it into the NEW DURATION and the latest completion date of all its child-tasks into the NEW END DATE.

![](../.gitbook/assets/image%20\(167\).png)

### KANBAN ISSUE TRACKING

Bug tracking and testing status reported bugs

![](../.gitbook/assets/image%20\(154\).png)

Drag and Drop:

* Main drag and drop flow: NEW – WIP – TESTING – DONE
* Cards from NEW column can be dragged to CLOSED, REJECTED or BACKLOG
* column RE-OPEN magnetic card can be pulled back to WIP BACKLOG can be dragged to WIP

Note: Only QC and DEV departments have the right to drag and drop in Issue Kanban

Update data:

* When dragging the card from TEST to DONE will automatically control **Last day update status** to the current date
* Manually enter **Testcase ID** when entering card to DONE or RE-OPEN

![](../.gitbook/assets/image%20\(232\).png)

### KANBAN REQUIREMENT

To track requirements and their status.

![](../.gitbook/assets/image%20\(233\).png)

Drag and drop:

* ALL columns - NEW - TODO - WIP - REVIEW - DONE: Common flow of a Requirement. Only employees of QC and DEV departments have the right to drag and drop cards according to this flow.
* NEW - CLOSED: Everyone has drag and drop permission. When the requirement is considered impractical and is denied approval and implementation.
* NEW - BACKLOG: Everyone has drag and drop permission. When the requirement is considered as not possible to do now and will be done in the near future.
* BACKLOG - WIP: Requirements that were included in BACKLOG in the past are now being implemented. Only employees of QC and DEV departments have the right to drag and drop cards according to this flow.
* WIP - DONE: indicates that the Requirement has been completed. Only employees of QC and DEV departments have the right to drag and drop cards according to this flow.

Update data:

* All sub-requirements in the table will change to the same state as the total requirement when dragging and dropping.

## USE CASES IN KANBAN

### To filter 1 column

**Step 1**. Click on the 3 vertical dots in the column you want to filter, select "**Filter column**".

![](../.gitbook/assets/image%20\(14\).png)

**Step 2.** Configure the filter according to your needs, then click "**Apply**" to apply the filter.

### To filter all columns

**Step 1**. To create a filter that applies to all columns in the kanban, click the filter icon in the upper right corner of the screen, then click "**Add**"

![](../.gitbook/assets/image%20\(159\).png)

**Step 2**. Configure the filter according to your needs and click "**Apply**" to apply. You can also give it a name and click the tick to save this current filter for reuse.

![](../.gitbook/assets/image%20\(31\).png)

### To view card details

Click on any card to see its details. Click the X button in the upper corner to exit detail view.

![](../.gitbook/assets/image%20\(16\).png)

### To edit card

To edit the card, go to View details then click "**Edit**". Or you can click the 2 dots in the corner of each card and click "**Edit**". After finish editing, click "**Save**" to save the changes.

![](../.gitbook/assets/image%20\(63\).png)

![](../.gitbook/assets/image%20\(117\).png)

### To drag and drop multiple cards

To drag and drop multiple cards at once instead of one by one, hold down the "**Ctrl**" key on your computer and left click on the cards you want to be grouped together to drag and drop. Multiple cards can be dragged from the same column or from multiple columns to another column.

![](../.gitbook/assets/image%20\(66\).png)
