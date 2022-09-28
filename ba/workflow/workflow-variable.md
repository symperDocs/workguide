# Workflow Variable

## Overview

Is a variable to get parameters from related modules: Document, User or are of nodes in workflow

Read more

{% hint style="info" %}
[Variable](https://simple.wikipedia.org/wiki/Variable)
{% endhint %}

To understand this chapter, you need to read [Formula Concept](../formula/untitled.md)

### JUEL

To use JUEL formula or SQL, Orchart, you need to know id [node](symper-bpm-notation/)

* id node: is an identifier ID for each node in a specific process

Ex: Requirement Workflow

<figure><img src="../../.gitbook/assets/image (14) (2).png" alt=""><figcaption><p>Node Create Req</p></figcaption></figure>

To know this node id, you need to click on that node, then look at the right side bar ([The attribute](workflow-editor.md#the-attribute-table))

<figure><img src="../../.gitbook/assets/image (13) (2).png" alt=""><figcaption><p>id node</p></figcaption></figure>

Every time a new node is created, the system will automatically create an ID

<figure><img src="../../.gitbook/assets/image (5) (2) (1) (1).png" alt=""><figcaption><p>ID that the system automatically creates</p></figcaption></figure>

Now, to get the value from the document in 1 node belonging to Workflow, we use ${`id_node_id_control}`

To find the id control of a [document](broken-reference/), you need to open the [document editor](../document/document-editor.md), you need to go to The Attribute of the first node and expand Task Action

<figure><img src="../../.gitbook/assets/image (1) (1) (1).png" alt=""><figcaption><p>From Reference</p></figcaption></figure>

Ex:

```
// ${tao_re_rq_id}
```

This formula will return the value when it is entered from the node with the ID is tao\__re_ and in control with ID is _rq_\_id

More Ex:

```
// ${id_node_executor_fullname}
```

This formula will give the name of the executor of that node

### Orgchart

Orgchart formula at workflow is often used to assign tasks for a specific role in ORG Chart or to check [flow](symper-bpm-notation/connecting-objects.md)'s conditions

More references

{% hint style="info" %}
[Org Chart Formula](https://docs.google.com/spreadsheets/d/1VmJGkKrz7aKdSPindQB6Bspg6PLwk4NMy0O\_MVK\_sGY/edit#gid=1311267643)
{% endhint %}

Ex:

<figure><img src="../../.gitbook/assets/image (7) (2) (1).png" alt=""><figcaption><p>Flow ConditionWe check whether the creator belongs to the Ba Back Manager department?</p></figcaption></figure>

```
// select case (select count(id) > 0 
     from role(ORG(symper).DPM_CODE(ba_back).MANAGER) 
     where id = '{tao_re_nguoi_lap}') 
     when 1 then 'true' else 'false' end
```

In this case, we check whether the creator belongs to the Ba Back Manager department? Get the value of nguoi\_lap field in Document and compare ID with BA Back Manager. If right, go to this branch

More Ex:

<figure><img src="../../.gitbook/assets/image (8) (2).png" alt=""><figcaption><p>Assignee</p></figcaption></figure>

```
// role(ORG(symper).DPM_CODE(ba_front).MANAGER)
```

This formula will return the results the Ba Front department
