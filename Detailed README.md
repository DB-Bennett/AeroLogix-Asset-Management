# Aero-Logix: A Practice in Logistics Data Management

### Project Overview

This project was designed as a hands-on exercise to practice the core skills required for a Logistics Support Specialist role at a government contractor. The primary objective was to simulate a real-world scenario involving Government Furnished Property (GFP) and to demonstrate proficiency in data management, inventory reconciliation, and documentation.

### The Problem

As a newly hired specialist, my first task was to perform a comprehensive audit of GFP for a fictional contract, "Project Pegasus." The challenge was to reconcile discrepancies between a contract's record of assets, the company's internal digital log, and a physical inventory count. This required meticulous attention to detail and a systematic approach to data analysis.

### Files and Structure

* `aero-logix-schema.sql`: Contains the SQL code for creating the database schema. This includes tables for `Locations`, `Assets`, and `MaintenanceLogs`. It also includes sample `INSERT` statements to populate the tables and example `SELECT` queries to perform analysis.
* `README.md`: This file, which details the project's purpose, problem, and solution.
* `Work_Log.md`: A separate document (or can be integrated here) that logs the steps taken and the findings of the reconciliation process.

### My Approach

1.  **Schema Development:** I first designed a relational database schema in SQL to logically organize the asset data. This included linking assets to their locations and maintenance history using foreign keys, a key step in building a robust data system.

2.  **Data Reconciliation:**
    * I began by comparing the `Pretend Contract` data with the `Digital Inventory Records`. I identified mismatches in the `Condition` of assets `PEGASUS-001` and `PEGASUS-005`. This highlights the importance of initial data verification.
    * Next, I reconciled the digital records against the `Physical Inventory Count`. This step revealed more significant issues:
        * The `Condition` of `PEGASUS-003` was different from the record (`Damaged` vs. `Used`).
        * A typo in the `Serial Number` for `PEGASUS-004` was found.
        * Asset `PEGASUS-005` was missing from the physical count.
        * Asset `PEGASUS-006` was an undocumented item found during the count.

3.  **Data Analysis:** Using the provided SQL queries, I was able to quickly extract meaningful information from the data, such as the total asset count per location and all assets in a "Used" or "Damaged" condition.

### Key Takeaways

This project reinforced the importance of:
* **Attention to Detail:** Small errors in a serial number can have a significant impact on compliance.
* **Proactive Problem-Solving:** Identifying discrepancies (like missing assets) and having a plan to resolve them is critical.
* **Structured Documentation:** Clearly documenting findings and your process is essential for maintaining a clean audit trail and communicating effectively with supervisors and government clients.
