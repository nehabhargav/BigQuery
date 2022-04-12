Hi !

This is a coursera guided  project by Ikechukwu Ogbuchi on BigQuery which actually works on BigData and performs visualizations.
Here you'll find all the insights about the course along with my learning. 

BigQuery Autodetects schema and input parameters
Important Information:

(1)  BigQuery is a Google Cloud service uses Google Cloud Platform. BigQuery Autodetects schema and input parameters
(2) The data used in this project is CoVID-19 Data in CSV file format. It contains 100,000 rows of COVID cases.
(3) The data set is taken from the website humdata.org
(4)Course Outcomes:

Task 1 - Project Overview - Working with BigQuery.
Task 2 - Navigating and Getting your Data into BigQuery.
Task 3 - Running SQL Queries with BigQuery.
Task 4 - Visualizing Big Data with BigQuery.
Task 5 - Saving reports, sharing and wrap-up.

(5) Steps:

1. Sign in to your google account
2. Go To your Google Cloud Platform -> Create New project -> Project Name -> Create.
3. To create a Query -> click Query -> Add your query 
           
----------(Query 1)----------
           
Select location, data, new_cases

from 'coursera-bigquery.coviddataset.covidtable'

LIMIT 1000

 
![ss1result](https://user-images.githubusercontent.com/53258421/162979192-b70453cf-b695-4f05-926c-d1d012fc36b8.png)

Fig 1. The result of the Query 1

----------(Query 2)----------
           
Select location,data, new_cases

from 'coursera-bigquery.coviddataset.covidtable'

WHERE date="2020-02-13"

LIMIT 1000

![ss1](https://user-images.githubusercontent.com/53258421/162978189-8814fef1-6be5-4bf4-abed-d8d7eaf805c1.png)


Fig 2. Writing the SQL query in BigQuery ( We obtain all cases from all locations for specified date mentioned in the Where Clause)

----------(Query 3)----------
          
           
Select location,sum(new_cases) AS total_new_cases

from 'coursera-bigquery.coviddataset.covidtable'

GROUP BY location

LIMIT 1000


![sumquery](https://user-images.githubusercontent.com/53258421/162979643-104157d4-fee5-4973-b366-856ca2cf403f.jpg)

Fig 3. Sum of new_cases for each location



The result generated thus is summoned as Views.
Therefore by querying our table we created downloadable Views.

----------------------------------------------------


(6) Here we will work on out Task 4 - Visualizing Big Data with BigQuery

----------(Query 4)----------

Select *

from 'coursera-bigquery.coviddataset.covidtable'  #your entire data is visible now

-----------------------------------------------------

**Visualization Steps:**


-> Click on Explore data 

-> We are going to visualise it using location & new cases 

![lcases](https://user-images.githubusercontent.com/53258421/162981449-ae869b99-88c0-41da-bdef-4bf5c84fdfde.png)

Fig 4. Take Locations and new cases.






->Then to Dimensions Add locations and to Metric add new_cases , new deaths

-> We will be visualising it using Pie Chart, Column chart, Tree maps.

![barplot1](https://user-images.githubusercontent.com/53258421/162983400-3c2e01d2-50b5-4400-b045-345a877b865a.png)

Fig 5. Barplot

![barplot2](https://user-images.githubusercontent.com/53258421/162983513-cbc45757-0f96-46f4-b489-40cb3b03f446.png)

Fig 6. BArplot2

![bubblechart](https://user-images.githubusercontent.com/53258421/162983622-99869fbc-625b-4fda-af03-1c4e7cfee090.png)

Fig 7. Bubblechart


![piechart](https://user-images.githubusercontent.com/53258421/162983696-cc123b72-7203-4127-9067-d44a7e8dbaf8.png)

Fig 8. Pie Chart

![treemap](https://user-images.githubusercontent.com/53258421/162983758-723bb2d1-cfd4-4002-8e2c-6168af18c10a.png)

Fig 9. Tree Map


(7) ** Sharing & Creating Reports **
-> Save Visualization
-> Share and add it to your report.





![report](https://user-images.githubusercontent.com/53258421/162987697-3e3bc06b-db7b-477b-a5eb-b1b2b9b35d98.png)

Fig 10. Creating Analysis report. 




<h1>Conclusion</h1>

1. BigQuery is a fully-managed, serverless data warehouse that enables scalable analysis. 
2. These task provided an insight for Google Cloud platform which makes handling large dataset, querying and analysing very quick & in an efficient manner. 
3. It also helps to creat many views , save it and then use it for further reports.












           
      
















