Hi !

This is a coursera guided  project by Ikechukwu Ogbuchi on BigQuery which actually works on BigData and performs visualizations.
Here you'll find all the insights about the course along with my learning. 


Important Information:

(1)  BigQuery is a Google Cloud service uses Google Cloud Platform.
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

![ss1](https://user-images.githubusercontent.com/53258421/162977208-25d2fffc-f5fd-467d-ad47-63849f5e7f74.png)

Fig 1. Writing the SQL query in BigQuery




![ss1](https://user-images.githubusercontent.com/53258421/162977219-60be41ea-9485-4561-a230-3a89dd85b632.png)

Fig 2. The result of the Query

----------(Query 2)----------
           
Select location,data, new_cases
from 'coursera-bigquery.coviddataset.covidtable'
WHERE date="2020-02-13"
LIMIT 1000

//Here we get all the cases from all the locations for the specified date mentioned in the Where statement.//

          xxxxxxxxxx
          
           
Select location,sum(new_cases) AS total_new_cases
from 'coursera-bigquery.coviddataset.covidtable'
GROUP BY location
LIMIT 1000

//Here we sum of new_cases for each location
![](image1.png)
<img src="images/image1.png" width="500" /> ![](images/image1.png)

The result generated thus is summoned as Views.
Therefore by querying our table we created views. You can also save your views.





(6) Here we will work on out Task 4 - Visualizing Big Data with BigQuery



Query

Select *
from 'coursera-bigquery.coviddataset.covidtable'.  #your entire data is visible now

Visualising Steps:


Click on Explore data 
we are going to visualise it using location and new cases 
Then to Dimensions Add locations 
and to Metric add new_cases , new deaths
We will be visialising it using Pie Chart, Column chart, Tree maps








           
      
















