# Symper WBS

### Training about Symper WBS

{% hint style="info" %}
[https://ywb69zeduvn.sharepoint.com/:p:/s/Symper347/EZ0IkUI2jh1OlM7OxCCvEOEBphLb86YuGC-6sgvfpPVo-w?e=mG5oEc](https://ywb69zeduvn.sharepoint.com/:p:/s/Symper347/EZ0IkUI2jh1OlM7OxCCvEOEBphLb86YuGC-6sgvfpPVo-w?e=mG5oEc)
{% endhint %}

### Overdue reason

Overdue reason table is used to declare the cause of employee's work delay.

**Step 1**. Each time an employee is unable to complete the work on time and has to change the plan start/end date, the employee must enter in the "Plan Start Date" and "Plan End Date" in the table before changing the current schedule and select the corresponding deadline delay cause.

![Overdue reason table](.gitbook/assets/image%20\(106\).png)

Note: Every time the assignee changes the deadline information outside the table, the status of the WBS will change to "Review" and need to be reviewed by the WBS Admin, ie the employee's Manager, and dragged to the "TO DO" column in Kanban.

**Step 2**. After entering all necessary information in the Overdue reason table, employees can re-enter information about their new deadline in the "Plan start date" and "Plan end date" fields outside the table.

![Changed deadline information outside the table.](.gitbook/assets/image%20\(86\).png)

### Kanban WBS

Kanban WBS serves to track and transfer work status of each person.

![](.gitbook/assets/image%20\(29\).png)

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

![](.gitbook/assets/image%20\(76\).png)

{% hint style="info" %}
[https://app.gitbook.com/s/-McNyP8y\_A8MZOZl5QPQ/others/kanban#1.-kanban-wbs](http://localhost:5000/s/-McNyP8y\_A8MZOZl5QPQ/others/kanban#1.-kanban-wbs)
{% endhint %}
