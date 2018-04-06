# Marketing-Cloud-Content-Reporting
A handful of queries and link tagging approach that will allow you to track content in Salesforce Marketing Cloud
Run these with a series of Data Extensions in order to end up with a final content report with categories and subcategories.

01 Newsletter Opens Past Month.sql is an overwrite query to a table with this structure

![First Table](tables/Newsletter%20KPI%20Past%20month.JPG)

02 Newsletter Sends Past Month.sql is an update query to the table above

04 Newsletter Bounces Past Month.sql is an update query to the table above

05 Newsletter Clicks Past Month.sql is an update query to the table above

06 Newsletter Unsubscribes Past Month.sql is an update query to the table above

09 Get Market an update query to the table above

## Content Bounces Table
We need this to pull all bounces for the past month so we can subtract them from Sent to get Delivered. It's basically just the _bounce data view.

03 Bounces Past Month.sql is an overwrite for the table below.

![Second Table](tables/ContentBounces.JPG)

## Newsletter Link Clicks from the past month
This is basically just the _click data view. we use it as an in between table to grab all of our clicks so we can count them later. The query also splits out the url varaibles into columns.
07 Newsletter Links Clicked Past month.sql is an overwrite for the table below

![Third Table](tables/NewsletterLinksClickedPastMonth.JPG)


