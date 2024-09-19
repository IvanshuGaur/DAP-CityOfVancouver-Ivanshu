# DAP-PortfolioProject-CityOfVancouver-Ivanshu
<h1>Descriptive Analysis of Gender Parity at City Of Vancouver using AWS</h1>
<h2>Project Overview</h2>
The City of Vancouver is improving its services with a <b>Data Analytics Platform (DAP)</b>, enabling better decision-making. My role in this project is focused on analyzing Gender parity.

The project provides insights into the <b>gender</b>, <b>payrates</b> and their <b>positions</b> for the years <b>2022</b> and <b>2023</b>.
<h2>Objective</h2>
The goal of the project is to <b>identify total number of males and females</b> working at City Of Vancouver in 2022 and 2023.


Dataset link: <a href="[https://www.google.com](https://opendata.vancouver.ca/explore/dataset/workforce-pay-rates-and-gender/information/?disjunctive.exempt_union&disjunctive.classification&disjunctive.position_title&disjunctive.data_category)">Workforce pay rates and sex</a>

<img src="https://github.com/IvanshuGaur/DAP-CityOfVancouver-Ivanshu/blob/main/Picture%201.png" alt="DAP" width="700" height="500">

<h2>Data Analytical Question Formulation</h2>
<h3>Goal</h3>
To analyze number of males and females working for City Of Vancouver in 2022 and 2023. How the trend has changed in a year.
<h3>Key Metric</h3>
Number of Males, Number of Females, Year
<h3>Methodology</h3>

<b>Data Collection and Storage</b>

AWS S3: The dataset was stored in two separate S3 buckets for the years 2022 and 2023, which ensured secure and scalable storage.

<b>Data Cleaning</b> 

AWS Glue DataBrew: The data was cleaned using DataBrew to address missing values, remove duplicates, and ensure consistency among both datasets.

<b>ETL Pipeline</b>

AWS Glue: I used AWS Glue to build an automated ETL (Extract, Transform, Load) pipeline, which enabled efficient data extraction from S3, transformation of the data, and loading it for analysis. 


<img src="https://github.com/IvanshuGaur/DAP-CityOfVancouver-Ivanshu/blob/main/Picture%202.png" alt="ETL" width="700" height="500">

<b>Data Analysis</b>

AWS Athena: I ran SQL queries to get the required output from the remaining dataset, in which i summarized the total number of males and females working. The result of the SQL query is shown in the image below.

<img src="https://github.com/IvanshuGaur/DAP-CityOfVancouver-Ivanshu/blob/main/Picture%204.png" width="700" height="500">

<h3>Data Vizualization</h3>

Excel: Data was vizualised using excel as AWS Quicksight was not accessible to the student account. The Histogram chart clearly states that male and female working at City Of Vancouver is nearly same in bith the years.

<img src="https://github.com/IvanshuGaur/DAP-CityOfVancouver-Ivanshu/blob/main/Picture%203.png" width="700" height="500">

<h3>Publishing and Web Hosting</h3>

AWS EC2: The analysis and results were published on a web server using AWS EC2 to make the findings easily accessible for stakeholders. The below screenshots show both, <b>Web server</b> as well as the <b>General Server</b>

<img src="https://github.com/IvanshuGaur/DAP-CityOfVancouver-Ivanshu/blob/main/Picture%205.png" width="700" height="500">

<img src="https://github.com/IvanshuGaur/DAP-CityOfVancouver-Ivanshu/blob/main/Picture%206.png" width="700" height="500">

<h3>Data Protection and Governance</h3>

AWS Key Management Service (KMS): KMS was utilized to apply encryption, to safeguard both data stored in S3 as well as the data transmitted over the networks. 
 Data Replication: It was the replication rules to make sure that a copy of data was created in different regions of AWS in case of failure in a particular region was experienced.

AWS Glue: The data was governed and managed through AWS Glue, where a tested zone was established to maintain data quality.

<h3>Data Monitoring</h3>

AWS CloudTrail: API calls and user activities across the AWS environment were monitored using CloudTrail, enhancing auditing and security measures.

AWS CloudWatch: CloudWatch tracked performance metrics and resource utilization, allowing me to monitor the health of services and ensure optimal performance.

<b>Data Insights and Findings</b>

The ratio of number of females and males working have been found to be approximately equal as seen in the histogram.

<h3>Tools and Technologies Used</h3>

<b>AWS S3</b>: data storage.

<b>AWS DataBrew</B>: Data cleaning and transforming .

<b>AWS Glue</b>: automating the ETL pipeline.

<b>AWS Athena</b>: To run SQL queries and analyze the data.

<b>Excel</b>: To visualize the data using charts and histograms.

<b>AWS EC2</b>: For hosting the analysis results on a web server.

<b>AWS Key Management Service (KMS)</b>: For encryption and data protection.

<b>AWS CloudTrail</b>: For monitoring user activities and API calls.

<b>AWS CloudWatch</b>: For tracking performance metrics and monitoring system health.

<h3>Deliverables</h3>

A report written in a clear manner and containing the overall information about methods, findings and recommendations. 
 Outlines and templates for easy interpretation of important information with the use of graphics.

<h3>Conclusion</h3>

I was able to assess the total number of males and females working at City Of Vancouver in 2022 and 2023 to ascertain information that will enable them to keep watch on the hiring methods. Thanks to AWS services employed in the project, its scalability and efficient performance was guaranteed along with the best security and compliance with data management standards.

