# Workflow Process

## Process Definition

A process definition is a Business Process Model and Notation (BPMN) 2.0 file that serves as a container for a process and its BPMN diagram. The process definition shows all of the available information about the business process, such as any associated subprocesses or the number of users and groups that are participating in the selected definition.

## Process Instance

A process instance is a specific occurrence or execution of a business process (Process Definition).&#x20;

For example, if making a cake is a process, the recipe is the process model. A process instance occurs each time a person makes a cake using this recipe.

In Symper Workflow, process instances can be started using events such as submitting a form, sending an email, or creating or uploading files, updating a document. Each process instance can be independently monitored and managed.

## Deploying a process definition

BPMN doesn’t have a notion of versioning. That is actually good, because the executable BPMN process file will probably live in a version control system repository as part of your development project. However, versions of process definitions are created in the engine as part of deployment. During deployment, Symper will assign a version to the ProcessDefinition before it is stored in the Symper DB.

Versions of Form definitions are created during deployment, where Symper will assign a version to the form definition before it is stored in the Symper Form DB.

For each Form definition, the following steps are performed to initialize the properties key, version, name and idThe process we’ll build is a very simple holiday request process. The Symper engine expects processes to be defined in the BPMN 2.0 format, which is an XML standard that is widely accepted in the industry. In Symper terminology, we speak about this as a [**process definition**](workflow-process-and-myitem.md#process-definition). From a _process definition_, many [**process instances**](workflow-process-and-myitem.md#undefined) can be started. Think of the _process definition_ as the blueprint for many executions of the process. In this particular case, the _process definition_ defines the different steps involved in requesting holidays, while one _process instance_ matches the request for a holiday by one particular employee.

## Job

A job is an explicit representation of a task to trigger process execution. A job is created when a timer event or a task marked for asynchronous execution is approached

A Job Definition provides details about asynchronous background processing ("Jobs") performed by the process engine.

Each Job Definition corresponds to a Timer or Asynchronous continuation job installed in the process engine. Jobs definitions are installed when BPMN 2.0 processes containing timer activities or asynchronous continuations are deployed.

## Process Instance Migration <a href="#__docusaurus" id="__docusaurus"></a>

When process definitions are updated with new versions, the question arises what should be done with already running process instances that are using older versions of the process definition. In case running process instances should be migrated to another process definition version, you can use the process instance migration features on the Symper Engine.

### Simple example <a href="#simple-example" id="simple-example"></a>

Let’s start with a simple example to explain the basics of process instance migration in the Symper Engine. In this simple example we use the following use case:

* There’s one process instance running with a process definition that has a key named simpleTasks and it consists of a start event - user task 1 - end event.
* The running process instance has an active state of user task 1.
* A new process definition is deployed with the same key (simpleTasks) and the process definition now consists of a start event - user task 1 - user task 2 - end event.
* The running process instance should be migrated to the new process definition.

