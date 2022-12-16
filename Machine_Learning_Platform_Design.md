# Design a Machine Learning Platform for a large tech company:

Relevant Questions to ask?
* What is the purpose of app/website?
* How will user interact with platform?
* What is the scale of use?
* Will we process decisions in real-time(online learning) or is it just the static model?
* Will the app be hosted over the cloud, or it will be present on private servers?
* Any security vulnerability issues or policies to be taken into account while designing such a system?
* Do the product needs to follow the microservices architecture i.e does it needs to be deployed over multiple places without changing the code structure?
* What is the scale of features, it needs to support? Does it require multiple models to give the right output?
* Do we have access to the HDFS data lake to process clickstreams?
* What is the scale of data needed to be processed?
* Do we need to create features on a real-time basis?
* Do we need to go towards Deep_Learning?

Managed Data: 
--> Provide a way to create, find, and share features and lables for machine learning.
--> If we have HDFS data lake to provide such, there should be a close integration with such HDFS datalake.
--> Scalable to thousands of data jobs(Petabyte scale data).
--> Provide data metadata:
	-Data-Metrics: Size, rows/columns, consumers, description, schema.
	-Quality-Metrics: Update frequency, Per Column(Missing Values, Variance), Percent of total missing data.
--> Incorporate data quality monitoring.
--> Provide online and offline data access.
--> Enable custom data transforms specifc to models.



	