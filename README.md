**Problem Statement:**

The department currently relies on the Signal application for daily communication and dissemination of business metrics, including actual vs. target figures and other important updates. Signal, however, can only be accessed via personal mobile phones due to company policy, and not on laptops.

The team is tasked with generating snapshots of data using conditional formatting in Excel. This process involves creating the visual representation on a laptop, capturing the screenshot, emailing it to a phone, and then sharing it on Signal. 

This workflow, from downloading raw data to updating formulas in Excel, creating conditional formatting, capturing screenshots, and finally emailing and sharing on Signal, is exceedingly time-consuming and inefficient.


**Solution:**

To streamline the current workflow and improve efficiency, I propose developing a data pipeline using SQL. The steps involved are as follows:

1. **Data Pipeline Development**:
   - Create a data pipeline using SQL to automate the extraction of required data from our databases.

2. **Scheduling Queries**:
   - Schedule the SQL queries using Airflow or our in-house scheduling tool, RAB, to ensure regular and timely data extraction.

3. **Excel Integration**:
   - Write SQL queries to retrieve the necessary data and connect them directly to Excel for seamless data import.

4. **Automated Conditional Formatting**:
   - Set up automated conditional formatting in Excel to generate reports with the desired visual presentation.

5. **Python for Visual Reporting**:
   - Use Python to capture and create images from the Excel reports, ensuring they are formatted correctly for sharing.

6. **Automated Email Distribution**:
   - Develop a script to automatically send emails with the generated reports attached to the designated email addresses.

7. **Signal Sharing**:
   - Upon receiving the email with attachments, automatically download the reports and share them on Signal.

This solution will significantly reduce manual effort, improve accuracy, and ensure timely distribution of business metrics and updates.
