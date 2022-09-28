# Common errors

## FileOVERVIEW

Document is one of four main element modules of symper platform. It was originally designed to provide access, analysis and storage data for your web apps. You can use simple drag & drop to design the form's appearance and basic SYQL to create a comprehensive data model, calculation and user experience logic.

## **FEATURE**

### **EDITOR**

#### Control <a href="#control" id="control"></a>

| Control          | Type   | Data type  |
| ---------------- | ------ | ---------- |
| **Label**        | View   | Text       |
| Imange           | View   | Img        |
| QRcode           | View   | Text       |
| Text put         | Input  | Text       |
| Rich text        | Input  | Text       |
| Number           | Input  | **Number** |
| Date             | Input  | Date       |
| Date time        | Input  | Date time  |
| Time             | Input  | Time       |
| Select           | Input  | T          |
| Combo bo         | Input  | Text       |
|                  | Input  | Text       |
| Radio            | Input  | Text       |
| Check box        | Input  | 1/0        |
| Percent          | Input  | Number     |
| User             | Input  | Text       |
| Input filter     | Input  |            |
| Primary          | Input  |            |
| Table            | Layout |            |
| Panel            | Layout |            |
| File upload      | Layout |            |
| Tab/page         | Layout |            |
|                  |        |            |
| Approval history | Report |            |
|                  |        |            |



* Width (px)
* Height (px)
* Text size
* Text color
* Hidden
* Read only
* Place holder
* Important

Validate

* Max length
* Min length
* Require
* Require change
* DB primary
* Table primary

Data

* Input data
* Default data
* Key cache in table
* Data array type
* Save data

Action

* Refresh data
* Quick submit

### **CONCEPT**

Document is a place to collect, store and provide input from end users to other Symper modules. For instance, document will be an input data resource for the BI module to get the data to show on the report.

### DISTINGUISH DOCUMENT DEFINITION & DOCUMENT INSTANCE

#### Document definition

Document definition is the document created after the BA creates it through Symper's Document module. After each time the end user enters and submits that document, the system will create a document instance that is exactly the same as the information that the user submitted.

The document definition enables you to access the attributes returned by the custom actions or connectors and use these attributes as an input or output within a process.

#### Document instance

A document instance is the data created by the application for which the structure is specified by the _document definition_. You can create a document instance whenever submitting a document or running a Workflow

