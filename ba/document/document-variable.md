---
description: >-
  Parameters that BA can use for logic generation when using document- Writer:
  Tannq
---

# Document Variable

## CONTEXT&#x20;

The `context` variable is used to check if the document is being executed in the workflow.&#x20;

To use the context variable in SYQL, the BA uses the `'{context}'` syntax to access the parameter. This variable has 2 values as follows:&#x20;

* `inWorkflow`: This value returned when the document is not being executed (submit or update) in the workflow.&#x20;
* `outWorkflow`: This value returned when the document is being executed in the workflow.

For instance:

```sql
SELECT case '{context}' 
when 'inWorkflow' then 'I/m in workflow' 
when 'outWorkflow' then 'I/m not in workflow' 
end
```

## ACTION&#x20;

The `action` variable is the variable used to check if the document is being submitted or updated.&#x20;

To use the action variable in SYQL, the BA uses the `'{action}'` syntax to access the parameter. This variable has 2 values as follows:&#x20;

* `submit`: This value is returned when the user is in the process of submitting text.&#x20;
* `update`: This value is returned when the user is in the process of updating the text.

For instance:

```sql
SELECT case '{action}' 
when 'submit' then 'submitting' 
when 'update' then 'Updating' 
end
```
