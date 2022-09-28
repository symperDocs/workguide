# Task Life Cycle

## Overview

The current Symper system of tasks has 2 unique hidden states as Assign and Complete. And cannot solve problems arising in complex reality

## Problem

* Demand for Asigin tasks for a group of people, user in the group can claim task and take responsibility for implementing task.&#x20;
* Demand for Re-assign tasks to others?&#x20;
* Demand for Delegate tasks to others?

## Solution

Use Flowable's Task Life Cycle model

## Task Life Cycle

![Task life cycle model](https://lh4.googleusercontent.com/yaSxOGZZERwka2AX8Am33WywGkAEYKqGaCsgE2ymOpMJ5Cfn2vjcl0qvXC6kQb7UwVu1-8yYQqmWT7u-6uEaIeVuHGAu5MpwFdbmXv-cTR1D1pJyIRjT-2oUYUzJ\_VDE-YQDcK1f)

Task Life Cycle model has 2 main components: **Stage** (circular boxes)and **Action** (on the flow)

* Stage is the state of tasks
* Action is user's action that will change the stage of the tasks.

Ex: When a task has no assignee (TASK has not delivered to a person), Task will have a status of **New**, When an user in the list of **candidates** of the task claim the task, the state of the task will be turned into **Assign**.

### List of Stages

| Stage     | Description                                                                                                                                                                                                                          |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| New       | Is a status when a Task is not assign for anyone and has not yet created a list of candidates                                                                                                                                        |
| Un Assign | Is a status when a Task that has created a list of candidates but has not assigned specifically                                                                                                                                      |
| Assign    | Is a status when a task assigned to a specific person and when performing the job or in case a person in the list of candidates to claim tasks to implement                                                                          |
| Delegate  | Is the status that Assignee Delegate the task to execute the task for another user. When completed Task, the delegate person will Resolve, Task will be returned to Assignee and Assignee that can confirm the completed task or not |
| Complete  | Is a status of a completed task                                                                                                                                                                                                      |

### List of Actions

| Action        | Description                                                             | Group of people are allowed |
| ------------- | ----------------------------------------------------------------------- | --------------------------- |
| Assign        | Assigns a task to a specific person                                     | Owner                       |
| Re Assign     | Re Assign a task to another user                                        | Owner                       |
| Set Candidate | Put one or a group of people attached to the candidate's position       | Owner                       |
| Claim         | User in the Candidate User group receive task                           | Candidate user              |
| Un Claim      | User cancel the receive task about Candidate User                       | Candidate user              |
| Delegate      | Assignee authorizes task for another user.                              | Assignee                    |
| Resolve       | User action is delegate to complete the task and resolve about assignee | Delegated User              |
| Complete      | Action completed task                                                   | Assignee, Owner             |

### Permission

|             | Owner                                             | Assignee                                  | Candidate User |
| ----------- | ------------------------------------------------- | ----------------------------------------- | -------------- |
| New         |                                                   |                                           |                |
| Un Assigned |                                                   |                                           | Claim          |
| Assgined    | <p>Re-assign/complete/</p><p>Unclaim/Delegate</p> | <p>Delegate/Re-assign</p><p>/complete</p> |                |
| Delegated   |                                                   | Resolve                                   |                |
| Completed   |                                                   |                                           |                |

### User groups

* Owner: As the owner of Task, who reserves the permission to complete the task and assign task for others
* Assignee: Is the person assigned to do the task
* Candidate User: As one or the group of people identified as the subject can participate in the job, Candidate User can Claim a task on to do if no one is assignee

#### Owner

Owner will have the following permission for work according to the Task Life Cycle model

* The permission to unclaim the task (when unclaim task, that job will return to the unsoign state. Can only unclaim in case there are many Candidate users participating in the task)
* Set Candidate (Add the Candidate List for Task or Remove the Candidate of Task - Only display the list of users with rights to the process and objects attached to Node in the process)
* Assign Task (the assign person will become an Assignee. There are 2 types of assigns that are complete and reporting task)
* Complete work

![](https://lh6.googleusercontent.com/GnL2KdcjEBVgCbFP4ABp15vGUE8ahvzExL2\_MrOUZPsC2zMqg2ucXGDkav4K0T1KlsCDmykJpDtPQ\_RNUru2Oz\_O\_H1348V4EB\_UXDUVStR-IdDGM4r44uIK4LxmL2sm78RQGBYJ)

#### Assignee



Type 1: Assignee is owner to deliver the job directly&#x20;

Type 2: Assignee Claim works on (this assignee is the user in the Candidate User group of the process, this user when Claim will be simultaneously Owner of the job)

For assignee assigned by Owner will have 2 cases that may occur:

* Owner assigns the job but does not deliver the permission to complete the job: For this case Assignee after completing the job must submit (resolve) again for Owner -> Owner will be the person who decides to complete the job or not to Process of implementing working flow
* Owner assigns the job and deliver the permission to the job to Assignee: For this assignee case after done and submit, the task will be completed and the process follows the next step.

For **Assignee Claim** work on **Un Assign** status will simultaneously be **Owner**: User will have full permission to work like Owner and

* Unclaim work
* Claim again&#x20;

Assignee's rights are assigned to complete the right: Assignee is assigned to complete the following rights:

* Delegate for others (the Delegate will become the assignee of Task)
* Permission to Set Complete Work

Assignee's rights cannot deliver the right to complete the task:&#x20;

* Assignee is assigned to complete the following rights:&#x20;
* Delegate for others (The Delegate will become the assignee of Task).

![](https://lh5.googleusercontent.com/iAwuUZTPwqWts-bPSgbUKtU78xTc\_It2Xfc3NYf5k49duTt9lVD3VvG7mzKqBpuMpSoVqkRl6NY62PG\_hEy2x4gfob7PasuhImlBRBFL1zChoZf5DHYcpilNSWnWcdME6HYTgvNz)

**Candidate user**

When a task only has Candidate User, Candidate User can Claim work, now User Claim will become Owner and Assignee's job.

User will have full permission for tasks like Owner

![](https://lh6.googleusercontent.com/Ox1fs1Svm9RVG6RgDx9lo8ltyWDzp4WMms6797SneJz2FO2MU\_DAaLC9URvTjZ\_MIotXA3tO82FmmoWOWpS6ZtLhGOCvD40HXg5NuT47RP\_POgUUkWshHC0l3ulK32GnY8x1D4Vh)

#### Approval case

* For approved tasks, only have Re Assign action
* When executing approval, the system automatically complete the job without passing the Set Task Complete step.

