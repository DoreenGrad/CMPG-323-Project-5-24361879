# CMPG-323-Project-5-24361879

Welcome to project 5. Monitoring and Reporting in power Bi. Version control like we did in project 4 is not possible with power bi and github.
I'll need to upload each iteration of the pbix file manually and then update my github readme file after each commit. 

I have made the first commit and it contains a pbix file. In the file there are two pages, Device Registration and Device Monitoring. Device Monitoring contains the following: 

![Screenshot (85)](https://user-images.githubusercontent.com/66521420/201081866-d0838d33-8d79-4091-bb1c-afb3cc9bb692.png)

I count the number of registered devices by their sub category ID and Zone ID in the two donut charts.
In the stacked column chart I compare the device status between inactive and active.
THese reports were requested in the rubric and indicate quantity of devices by device name.

On the Device Registration page I have the following:

![Screenshot (87)](https://user-images.githubusercontent.com/66521420/201082609-31a45e1b-4647-4b15-b694-4753b17db842.png)

Here I count sub category ID be device name in the stacked bar chart. And we have two time oriented reports. In the stacked column chart we count registered devices by their zone ID's and determine in which year they were installed/registered. The report at the top is fun to look at, here I used a timeline slicer, combined with a line chart. The timeline slicer works better when there are more datapoints but you can see the just of it here. It represents months, quarters and years...but can go down as far as days. It compares those three time dimensions to the line chart underneath which counts the number of registered device ID's by year.

Commit number 2. This commit contains the High Level Metrics page. Here I used tables and two line and clustered column charts. The visual looks cool but the high level metric come in with the week calculation to calculate the number of weeks in a year and then the weeknum measure that gets used as a tooltip to give important information when hovering over the charts. The week calculation makes use of DAX  to get the week in which a device was installed/registered or in this case the device ID by category ID and device ID by zone ID. The tables are used to represent the relationships between the entites'datasets in the model view and to show off the calculation of week and the measure weeknum which I used in the charts as a tooltip. I had to create relationshps in order to set up the visuals and tables metrics I provided in my report. I also had to transform the data in the csv file because the column headers were out of sorts and the naming of them was inconsistent. I also had to change the attributes of sub category and category because they seemed to be confused. I also removed category ID attribute from device entity and replaced it with sub category ID attribute. 

High level Metrics page:

![Screenshot (99)](https://user-images.githubusercontent.com/66521420/201088843-0a84767d-fd02-4a52-8703-727052d173b5.png)

Entity relationships/ datasets relationships on the model view:

![Screenshot (92)](https://user-images.githubusercontent.com/66521420/201089024-da74b38b-de83-4d0c-bf0e-b82f81ac74a3.png)

Here I used the power query editor to transform the data from the csv file:

![Screenshot (97)](https://user-images.githubusercontent.com/66521420/201091601-b5e8a828-cf95-4101-bd1a-09f51512a128.png)

Here is an example of one of the changes made in power query editor. I had to replace category ID with sub category ID because the data didn't make sense the way
it was setup. 

![Screenshot (95)](https://user-images.githubusercontent.com/66521420/201092412-debe5e37-963e-4eaf-9692-0af99d5bda22.png)

Here is my week calculation:

![Screenshot (93)](https://user-images.githubusercontent.com/66521420/201092530-e0b79618-da24-49d5-b4a7-919c2dd62bd3.png)

Here is my weeknum measure which is also a calculation (average) and used as a tooltip in the charts.

![Screenshot (94)](https://user-images.githubusercontent.com/66521420/201092744-b2ed25fd-9b64-496e-872a-7223904e42db.png)

Last but not least, I have published my report and dataset and the csv file that I used for my dataset onto power bi service. I have also published it from power bi
service to github in an attempt to do version control. Instead power bi service asked me to use a paid version of which I now have a 60 day free trial to do this. It
didn't turn out how I thought the instructions were instructing me, instead it created a github workbook on power bi service. I'll include the link in this readme so that you can check it out if you want. 

![Screenshot (100)](https://user-images.githubusercontent.com/66521420/201094971-88f05d85-0f28-4653-85a7-f40be56b02c1.png)

![Screenshot (101)](https://user-images.githubusercontent.com/66521420/201094999-24498ee0-83f8-4671-b350-90ef3ff5d6b4.png)

![Screenshot (102)](https://user-images.githubusercontent.com/66521420/201095049-bd43d3bc-a8c3-4c1b-9fa5-52cb573d881c.png)

I have also added filters to this report which allows the user to filter any data they deem neccessary. I have include universal fiters for device name/ID, Zone ID 
category ID and timeline filtering. Below is a visual from my report representing this:

![Screenshot (105)](https://user-images.githubusercontent.com/66521420/201104107-b41a773a-6569-4073-82fd-efe64d8a85fe.png)

![Screenshot (106)](https://user-images.githubusercontent.com/66521420/201104149-f21412da-969e-458d-8a77-8eaccce200ef.png)

https://app.powerbi.com/groups/051f33aa-11fd-4459-9988-a3c72f8a8b40/list
https://app.powerbi.com/groups/051f33aa-11fd-4459-9988-a3c72f8a8b40/reports/c6bae9ed-570b-4d60-9676-c9cdc3100089/ReportSectioncd021c7c43ad28778baf




