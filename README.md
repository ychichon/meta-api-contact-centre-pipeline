# Meta API Integration – Contact Centre Data Transfer

This internal automation project replaced a manual process by implementing a data pipeline that transferred campaign data from Meta into our contact centre system and SQL Server database.

##  Project Overview

Using **Graph API** and **Azure Logic Apps**, I retrieved complex, deeply nested JSON data. One of the key challenges was handling its irregular structure, which I addressed through custom parsing and mapping logic.

The Logic App was scheduled to run every 30 minutes, as requested by the call centre team, and included built-in control checks. I used **Excel** for testing and validation during development, and implemented **Azure Monitor and Alerts** to track the pipeline in production.

In addition, I developed a **Power BI dashboard** for the fundraising manager to monitor campaign engagement and performance, providing real-time insight into results.

>  *Note: This project involved internal systems and confidential data, so files are not publicly accessible.*

---

##  Tools & Technologies

| Tool / Technology        | Purpose                                                              |
|--------------------------|----------------------------------------------------------------------|
| Graph API                | Retrieving Meta ad campaign data                                     |
| Azure Logic Apps         | Workflow orchestration, control logic, and scheduling                |
| JSON Parsing & Mapping   | Handling deeply nested structures and aligning with API schema       |
| Call Centre API          | Delivering structured data to operational systems                    |
| SQL Server               | Internal data storage and reporting                                  |
| Excel                    | Validation and QA during development                                 |
| Azure Monitor & Alerts   | Workflow monitoring and issue detection                              |
| Power BI                 | Internal dashboard for fundrasing team to monitor campaign engagement and performance                |

---

##  Power BI Report

Created a dashboard for internal use by the fundraising team, showing:
- Daily engagement and reach by source (paid vs organic)
- Performance trends across the campaign lificycly
- New vs returning contacs
- Real-time campaign tracking for informed decisions

*(Visual previews and logic diagrams available upon request.)*

---

##  Author

**Yolanda Chichón Parra**  
Data & BI Developer  
[LinkedIn Profile](https://www.linkedin.com/in/yolanda-chichon-parra)

---

##  Want to Know More?

This is a private, internal project. If you'd like to learn more about my work with API integration, automation, or Power BI storytelling, feel free to contact me. I’m open to freelance, contract, or remote data roles across the UK and Europe.

