# 🛠️ Data Migration Project: Microsoft Dynamics 365 ➡️ Salesforce

This project documents the complete process I followed to migrate data from **Microsoft Dynamics 365** to **Salesforce**, using **Salesforce Data Loader** as the primary tool. The migration process was carried out in six key phases to ensure a smooth, accurate, and efficient transition of business-critical data.

---

## 🔹 1. Planning

The first step in the migration process involved thorough planning. I began by engaging with stakeholders to understand which data needed to be migrated and which could be archived or excluded. I then documented the data model of Dynamics 365 to understand how it aligned with Salesforce's schema. During this phase, I created a high-level migration strategy that included timelines, data sources, tools, and responsibilities. The goal here was to ensure everyone was aligned and prepared before any data movement began.

---

## 🔹 2. Profiling

Once the plan was in place, I moved on to data profiling. This involved digging into the actual data sets to assess quality, volume, and structure. I used tools like Excel and simple queries to analyze fields, identify inconsistencies, check for duplicates, and highlight any null or improperly formatted values. At this stage, I also created a detailed mapping document — matching fields in Dynamics 365 to their counterparts in Salesforce — and identified any transformations or adjustments that would be needed prior to migration.

---

## 🔹 3. Data Cleansing

With profiling complete, I turned to data cleansing. This was a critical step to ensure that the data being migrated was clean, consistent, and reliable. I removed duplicate records, standardized formats (such as phone numbers and dates), and filled in any missing values where possible. I also normalized values across picklists and ensured that lookups or relationships would not break during the transfer. Cleansing was done both manually (in Excel) and through scripts, depending on the volume and complexity of the data.

---

## 🔹 4. Execution

Next came the execution phase — the actual data migration. Using Salesforce Data Loader, I imported the cleansed and prepared data into Salesforce. I followed the proper object hierarchy to maintain relationships, starting with foundational objects like Accounts and Contacts, then moving to related records like Opportunities, Cases, and Custom Objects. I monitored logs for each batch upload to ensure successful execution, and where errors occurred, I resolved them and re-ran only the affected batches. This iterative, controlled approach helped reduce risk and avoid major data issues.

---

## 🔹 5. Audit

After the data was migrated, I conducted a comprehensive audit to validate that everything transferred correctly. This included checking row counts, confirming relationships were preserved, and comparing sample records between the source and target systems. I created summary reports showing which objects had been migrated, how many records were moved, and what error rates (if any) occurred. This step was important to build confidence in the accuracy and completeness of the migration.

---

## 🔹 6. Data Integrity

The final step focused on ensuring data integrity post-migration. I worked closely with business users to spot-check key records and validate field-level accuracy. I also verified that automations (such as workflows, validation rules, and triggers) were not unintentionally disrupted by the new data. In this phase, I documented all findings, resolved any integrity issues, and obtained final stakeholder sign-off. This confirmed that the data was not only migrated successfully, but also functioned as expected in its new Salesforce environment.

---

## ✅ Outcome

This structured approach resulted in a highly successful migration from Dynamics 365 to Salesforce. The project met all its objectives:
- Data was cleansed and standardized.
- Migration was completed with minimal disruption.
- Stakeholders confirmed system readiness.
- Post-migration support was minimal due to proactive planning and validation.

---

## 🧰 Tools & Techniques

- **Salesforce Data Loader** – Used for importing/exporting data in bulk.
- **Excel / Google Sheets** – Used for mapping, cleansing, and validation.
- **Manual QA** – Spot-checks and data validation.
- **Stakeholder Reviews** – Ensured business confidence and alignment.

---

