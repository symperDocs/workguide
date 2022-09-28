# Workflow Editor

Workflow is a method that describes the steps of a planned business process from end to end. It allows for easier communication and collaboration to reach the goal of an efficient process that produces a high-quality result. To create or edit a workflow, we use a workflow editor. In the workflow editor, there are 3 main elements each has different functions: the toolbar, the palette, and the attribute table as below:

<figure><img src="../../.gitbook/assets/image (30) (1).png" alt=""><figcaption><p>Workflow editor</p></figcaption></figure>

### **THE** TOOLBAR

The toolbar is on the top side of editor, offers a number of actions, some of them only affecting the currently opened model while others have a more impact.

| **Name**         | Icon                                                                                                                                                                                                              | Description                                                                              |
| ---------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------- |
| Undo             | ![](https://lh4.googleusercontent.com/hLrhk7oTx9ZX8F9mcHmn83SKfnr0etuVyEUHZ2if9YCqKWQSAMyqK\_wjjKiQR6c3PVPVE8qrZiMQGPccwISPLwMFrMHoDw7opZMANvrPG0qpFlw6AtITj4-bLZGaa4VRR4YqfYRY=s0)                               | Undo the previous action.                                                                |
| Redo             | ![](https://lh3.googleusercontent.com/iMfsUtGABm2DP4OBwhiPobHYu0GK1bLh5r3efZkkA6StausfSQfD3xI1cJ-JEWU4AbEVley-8hqiZ93Pll3U9NKg\_G29TiDoXay9I7CyYpDYJ4p1rCjKBWwCptB1gf5TrpM40rsl=s0)                               | Redo the most current action.                                                            |
| Zoom in          | ![](https://lh5.googleusercontent.com/\_XvY1W\_deS3U01uekFg6RY8sa4T4w5ipyqTMY8WpqxpqF6WXGbI4H2vLTFdfhooMwiD2rAdOEGmAvtC2Fj7QRitzoAztgqYOgvz\_JIOfl7OC2\_y8Fm8mMZugwURJNLUIf-s7AANQ=s0)                            | Make the workflow model appear much larger and nearer, or much smaller and further away. |
| Zoom out         | ![](https://lh6.googleusercontent.com/ImQ\_7RWuXlZ11NFtRb0Y2O5MFlSSn\_frI1NOlsad4C5dmhDv2o82R6O2ZA2eS\_4z4pVeb8uZe0eZvHs0OXQGDIkiUBzkQRHT5bxBwWT3Zt8g16FulEOnoaCjVJIYxaURRxHroT7S=s0)                             | Make the workflow model appear much smaller and further away                             |
| Focus            | ![](https://lh5.googleusercontent.com/K\_wCgjKJjs6\_HzY6L9nBbDwnOP7AbdOFZeLjgWsJIKwkVZU4nwJ6ZedSXBNZ0Jh9I5uLUuwqd9l6waqkPAdsiupx\_K2U8lMUwhyh2IQkPBVmAGjLhylKFyCRV\_HtfwYHqQDYOp0z=s0)                            | Focus on the centre of the currently opened model.                                       |
| Save as image    | ![](https://lh6.googleusercontent.com/BJ31AotcfyZfgXvTkgWW7X11JPDN4-aQSPR9D8F91nqZIREqCUTJNTlCqT-kLWwAZcp8XKMs-bhOo3tYoxjFSHqnja8wAn6flu-IQF7-QCAuJcjpgK-wRiKtbZXJizzsUvqqcy6B=s0)                                | Download the currently opened workflow model as an image.                                |
| Save as .bpmn    | ![](https://lh4.googleusercontent.com/KDyXtxTabhHcM334qw-4IRbpOyVXFwSbU1Nd0m6v2rUEFlQvwohKrUKDi86YMBuy-arYoCB9VfFi0MlUAyhBSkYYnPFlGbmCd3YdZgIbhoNb35rnYqUHAcKeJFNJBkR-SPn6U77K=s0)                                | Download the currently opened workflow model as a bpmn file.                             |
| Validation check | ![](https://lh5.googleusercontent.com/QEVIMWBiXZGsmzohvuqbTjb0BnmK1DkDWIkE\_7OLC7WzglD8UBXwRTmzGwNHixPaBMEV9mQ-\_BUogROwwe9zhmYVMCNZpATR9tL6-Kmf3K4Ot1wbKUjtdZc55EtfYBc3cDCVb8X4=s0)                              | Check whether the current workflơ model is valid for saving or not.                      |
| Save             | <img src="https://lh3.googleusercontent.com/sSUPB11tJ8ptl-28UefsGqa6DpIh3hvoPvH5QLVGD7IcSBiGHGck7XQX7kaId45R_U3rAVaoXONCT7rfWXhtYJa6MJ_SmTRnyZV0cFbRnLq4VohGi7Kr3RI7myu_VQjD0sDagJBf=s0" alt="" data-size="line"> | Save the currently opened workflow model.                                                |

### **THE PALETTE**

The palette is on the left side of the workflow editor, it contains actions that allow we can create or edit any element in the workflow.

| **Name**                  | Icon                                                                         | Description                                                                                                                             |
| ------------------------- | ---------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Hand tool                 | <img src="../.gitbook/assets/image%20(155).png" alt="" data-size="original"> | To drag one node to another position in the workflow editor                                                                             |
| Lasso tool                | ![](../.gitbook/assets/image%20\(120\).png)                                  | To drag an interval to another position in the Workflow editor                                                                          |
| Create/remove space tool  | <img src="../.gitbook/assets/image%20(152).png" alt="" data-size="original"> | To create or remove space from any position. It can make 2 node's space further or closer                                               |
| Global connect tool       | <img src="../.gitbook/assets/image%20(161).png" alt="" data-size="original"> | To make connections between elements in the workflow                                                                                    |
| Start event symbol        | <img src="../.gitbook/assets/image%20(88).png" alt="" data-size="original">  | Signals the first step of a process.                                                                                                    |
| Intermediate event symbol | <img src="../.gitbook/assets/image%20(217).png" alt="" data-size="original"> | Represents any event that occurs between a start and end event.                                                                         |
| End event symbol          | <img src="../.gitbook/assets/image%20(162).png" alt="" data-size="original"> | Signals the final step in a process.                                                                                                    |
| Create gateway            | <img src="../.gitbook/assets/image%20(58).png" alt="" data-size="original">  | Creates a new gateway that is used to check how a process is going                                                                      |
| Create task               | <img src="../.gitbook/assets/image%20(246).png" alt="" data-size="original"> | Creates a new node of task                                                                                                              |
| Create subprocess event   | <img src="../.gitbook/assets/image%20(224).png" alt="" data-size="original"> | Creates a subprocess event                                                                                                              |
| Data object reference     | <img src="../.gitbook/assets/image%20(109).png" alt="" data-size="original"> | Represents data placed into the process, data resulting from the process, data that needs to be collected, or data that must be stored. |
| Data store reference      | <img src="../.gitbook/assets/image%20(77).png" alt="" data-size="original">  | Represents the ability to store or access data that’s associated with a business process.                                               |
| Create Pool/ Participant  | <img src="../.gitbook/assets/image%20(128).png" alt="" data-size="original"> | Creates pool that defines a process or organization                                                                                     |
| Create group              | <img src="../.gitbook/assets/image%20(2).png" alt="" data-size="original">   | Allows to organize multiple tasks or processes into a group, make it more specific how each of those steps is completed.                |

### **THE ATTRIBUTE TABLE**

The attribute table is on the right side of the workflow editor, it contains the general and detailed information of the Workflow

<figure><img src="../../.gitbook/assets/image (2) (1) (2).png" alt=""><figcaption><p>The attribute table</p></figcaption></figure>

**General:**

* Name: name of the Workflow
* Description: to describe the present Workflow

**Detail:** has detailed information on the full Workflow, helps users can be more specific about the workflow's details, however the following are some of the most often used components:

<figure><img src="../../.gitbook/assets/image (6) (1).png" alt=""><figcaption><p>Detail section in Workflow editor</p></figcaption></figure>

* _**Display text for the process instance**_: It displays the name of the workflow that will be displayed in My item, making it easier for users to know what that workflow is for.
* Data objects: defines a structure of the data
* Signal definitions:
* Message definitions:
