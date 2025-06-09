# Meta API Integration – Azure Logic App JSON

This repository contains a Logic App definition (in JSON format) used to automate the ingestion and transformation of Meta lead campaign data into internal systems, including a contact centre API, Azure SQL Server, and Azure Blob Storage.

##  Project Context
This Logic App replaced a manual process of retrieving, transforming, and distributing lead data generated from Meta ad campaigns. It was designed to:

- Ingest raw engagement data from Meta (Graph API)
- Parse and transform deeply nested and irregular JSON
- Update internal SQL Server databases
- Deliver structured payloads to an external call centre API
- Track metadata using Azure Blob Storage
- Run reliably on a 30-minute schedule with monitoring and control logic

>  Note: This Logic App file includes **dummy connections and redacted tokens** for security. It is intended for demonstration only.

##  Key Components

| Component                | Purpose                                                                 |
|-------------------------|-------------------------------------------------------------------------|
| **Graph API**           | Retrieve Meta campaign lead data, including paid and organic engagement |
| **Azure Logic Apps**    | Orchestrate workflow logic and scheduling (every 30 minutes)            |
| **JSON Parsing**        | Handle nested structures like `field_data` dynamically                  |
| **Azure SQL**           | Insert transformed lead data into internal reporting tables             |
| **Call Centre API**     | Send structured lead data to operational teams                          |
| **Azure Blob Storage**  | Track `last_pull_time`, `last_id`, and run metadata                     |
| **Control Logic**       | Skip or proceed based on data freshness and count checks                |
| **Excel (external)**    | Used during development for data QA and validation                     |

##  Highlights

- **Dynamic JSON parsing**: Adapted to irregular field positions and missing values using `if()` logic.
- **Reusability**: Variables and modular updates allow for flexible changes in schema and data flow.
- **Monitoring**: Control files and counters stored in Blob Storage enabled auditability and retries.
- **SQL integration**: Data was mapped to an external SQL table using Azure API connections.

##  File: [`meta-logicapp-snippet.json`](./meta-logicapp-snippet.json)
This is a simplified excerpt of the Logic App workflow definition, highlighting dynamic JSON parsing, conditional control checks, and Azure Blob Storage logic.

##  Credentials
All API keys, tokens, and resource identifiers have been **redacted** or replaced with placeholders.

## Author
**Yolanda Chichón Parra**  
Data & BI Developer  
[LinkedIn Profile](https://www.linkedin.com/in/yolandachichon)

---

>  **Interested in automation and API integration?** Feel free to contact me if you'd like to collaborate or discuss similar automation projects. I'm currently available for roles in the UK and across Europe.
