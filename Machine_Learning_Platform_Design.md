# Design a Machine Learning Platform for a large tech company:

**Relevant Questions to ask?**
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

**Managed Data:** 
* Provide a way to create, find, and share features and lables for machine learning.
* If we have HDFS data lake to provide such, there should be a close integration with such HDFS datalake.
* Scalable to thousands of data jobs(Petabyte scale data).
* Provide data metadata:
	* Data-Metrics: Size, rows/columns, consumers, description, schema.
	* Quality-Metrics: Update frequency, Per Column(Missing Values, Variance), Percent of total missing data.
* Incorporate data quality monitoring.
* Provide online and offline data access.
* Enable custom data transforms specifc to models.

![image](https://user-images.githubusercontent.com/42828760/208073292-1b64a075-b6da-4dee-93fb-981b5ee8dc5f.png)

* An API can be used to trigger operations over feature Space.
* Data can be stored in Example Store.

Questions to ask?
* How can one orchestrate daily jobs from the data lake to the featured Store?

**Updated with managed model, monitoring and experiments:**
![image](https://user-images.githubusercontent.com/42828760/208108311-cc87c444-b504-473b-8c18-d0224caab07d.png)
Points to take care:

Managed Models:
 * Support online model hosting.
 * Support Batch Inference.
 * Support model training with recent features and labels.
 * Support Potentially tens to thousands of requests per second.

Managed Experiments:
 * Support Experiment Creation.
 * Support Viewing in progress and historical experiments and experiment results.
 * Enable frequentist/Bayesian A/B testing as well as multi-armed bandits.
 * Support Experiment Stoppage within minutes.

Managed Monitoring:
 * Interface to see history of model outputs.
 * Interface to see how customer responds to model outputs.
 * Drift Detection(Drop in accuracy etc).







	
