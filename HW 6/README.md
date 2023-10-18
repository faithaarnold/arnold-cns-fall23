# 1/c Faith Arnold - CNS Homework #6 - 17 October 2023
## Splunk Training

For this section of the homework, I completed the Intro to Splunk course. This course goes over the basics of Splunk, delving into creating reports and dashboards and how to use the Splunk search processing language. The topics covered in the beginnning of the course include the components and basic functions of Splunk, how to use Splunk, define apps, and understand user roles, utilizing the Search & Reporting app, and navigating the Splunk Web interface. Moving on to searching and data processing, you'll learn about running basic searches, setting time ranges, saving results, and understanding the contents of search results. The exploration continues with refining searches and understanding timestamps in events, using the Search Processing Language for advanced search techniques, including wildcards, case sensitivity, booleans, and special characters. I delved into the anatomy of Splunk's search language, its components, and best practices for writing searches. Knowledge Objects are introduced, covering categories like data interpretation, classification, enrichment, normalization, and data models. Lastly, I learned how to create reports, edit them, use transforming commands for visualizations, and build dashboards. These topics provide a comprehensive overview of using Splunk for data analysis and management

The certificate of completion for the Intro to Splunk course has been pushed to this GitHub repo under the HW 6 folder.

## SIEM Tuning

### Windows Event ID Exclusion

The Windows Security ID I chose to do was 4720: A user account was created. This event ID shows the properties of the account when it was created, and is logged for both local SAM accounts and domain accounts. I chose this event because it does not have a heavy influence on the system's security, and in our AD setup, we should already know when user accounts are created.

### Updated inputs.conf file

The updated inputs.conf file containing the group's chosen blacklisted event ID's have been pushed to this GitHub repo under the HW 6 folder.

The file can be seen along with the file location in the screenshot below.

![image](https://github.com/faithaarnold/arnold-cns-fall23/assets/90394310/b06a707c-1407-4670-8f33-053b5d43ff92)
