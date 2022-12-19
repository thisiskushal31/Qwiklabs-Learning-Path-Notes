#### Innovating with Data and Google Cloud

Business data is not a new term. Businesses have leveraged information about performance and operations for centuries to make decisions. Traditionally, data analysis could take days or months, is often incomplete, and complex reports were often done by specialized teams. Cloud technology disrupts traditional data analysis. Data can now be consumed, analyzed, and used at speed and scale never before possible.

In fact, businesses can now leverage cloud technology to ingest data in real time to train machine learning models and to take action.  

In this course, we're going to explore how businesses can better use data in their digital transformation journey.

***In Module 1***, I'll define data and its role in digital transformation. I'll identify where you can find data and how you can create new insights by combining different datasets.

***In Module 2***, I'll examine the differences and similarities between databases, data warehouses, and data lakes. I'll offer use cases for each and some relevant Google Cloud solutions for getting the most value from your data.

***Finally, in Module 3***, I'll look at machine learning and artificial intelligence. I'll highlight key opportunities for applying ML in any business and cover common Google Cloud ML and AI solutions that you can start using right away. Throughout the course, what I want you to remember is you don't have to be a data scientist or technical expert to do data analysis or to use machine learning.

In fact, with the right cloud tools, data is now accessible in new ways. Anyone in your organization can unlock the value of data to enable digital transformation.

#### Module 1 (The Value of Data)

Businesses now have access to data like never before. This includes internal information, data from inside your organization, and external information, customer and industry data. For example, as organizations have digitized their operations, all kinds of business data has become available, such as financial information, logistics data, production output, and quality reports. Businesses also have access to new kinds of data about their customers. Consider digital interactions such as the length of time a user spends on a web page or reaction to a social media post. These are totally new and very rich sources of information about customer behavior. 
So for example, shopping mall previously we used camera check theft activity but now we can use those cameras to monitor expression towards the product are you inside a mall and optimise it to make better sales.
 
Above is an example of data collected for delivery company you should deliver food and even its applicable for the larger cargo delivery in terms of User data, Corporate data, Industrial data.

So, using User-Data and Industrial-Data *(mostly in Structure and Unstructured Data)* we can optimize what Corporate data being obtained and used/optimise digital transformation.

##### Type of data

- **Structured Data**: Structured data is highly organized. Examples include customer records consisting of names, addresses, credit card numbers, and other quantitative data. Structured data can be easily stored and managed in databases.
- **Semi-Structure Data**: Semi-structured data is data that does not conform to a data model but has some structure. It lacks a fixed or rigid schema. It is the data that does not reside in a rational database but that have some organizational properties that make it easier to analyze. With some processes, we can store them in the relational database. 
- **Unstructure Data**: Unstructured data has no organization and tends to be qualitative. Examples of unstructured data can include word processing documents, audio files, images, and videos. This data can be stored as objects. An object consists of the data itself, a variable amount of metadata, and a globally unique identifier. Some unstructured data can be stored in a format called a BLOB. This stands for Binary Large Object. Images, audio, and multimedia files can all be stored as BLOBs.

##### Important data considerations

Capturing, storing, and analyzing vast amount of data is key to adopting Cloud technology. But handling this volume and diversity of data comes with its own ethical considerations and requires alternative ways of thinking about security. Google believes that capturing and managing data demands responsibility and accountability. Not all information that can be captured should be captured. In other words, businesses are accountable for making responsible decisions about which data they collect, store, and analyze. This also extends the data that businesses already own. In this case, it's essential to examine who has access to the data and how they'll be using it.

First, consider the source of the data, how it's being collected, and where it's stored. If it's personal or sensitive data about a customer or an employee, it needs to be securely collected, encrypted when stored in the Cloud, and protected from external threats. Additionally, only a subset of users should be granted permission to view or access the private data. Data security and privacy becomes more complex in a global economy. Let me explain where this can be particularly important. Suppose, for instance, you want to use thousands of lung X-ray images to train an ML model to automatically identify tumor markings in new patient X-rays. What you need are the X-ray images. This is the relevant data. What's not relevant is patient's personal data. You need to ensure that any source data about individuals such as names or addresses is omitted or redacted. There's also some information that is not personally identifiable and should still not be included in the modeling for ethical reasons.

#### Module 2 (Data Consolidation and Analytics)

Businesses that leverage data effectively can improve efficiency and productivity, deliver fresh, personalized customer experiences, and create new business value and how you can combine them to generate insights and take intelligent action.

In particular, I discussed the different types of data that businesses can access, and how you can combine them to generate insights and take intelligent action. The way that data is collected, stored, and managed is foundational to what you can do with it. In this module, I'll start by considering where data is now and the benefits of migrating your data to the Cloud.  

When you store your data on-premises, you're responsible for the IT infrastructure that supports the collection, security, and processing of that data. You're also responsible for maintaining and expanding the capacity of your IT infrastructure. This can be expensive and time-consuming. It's also difficult to scale quickly. If you have limited storage space, then you risk missing opportunities to gain insights with new data.

You also risk downtime. Imagine that you launch a mobile app and don't accurately predict demand. A lot more people download and use it than you expect. Your infrastructure isn't set up to absorb that much data that fast. As a result, the app freezes or crashes, resulting in dissatisfied users. With Cloud, you can rent space from public Cloud providers like Google Cloud. This means that your data storage and compute powers are elastic. It can scale up or down as the data you take increases or decreases.

*These are many solutions for data storage:*

- *Cloud database or Database* : A database is an organized collection of data generally stored in tables and accessed electronically from a computer system. Companies typically use a database to keep track of their basic online transactions, provide information that will help the company run its business efficiently, or help managers and employees make better decisions. For example, a hotel booking site would use a database for their customer transactions.If a person books a room for a night, that data is captured in the database, and the room availability is updated in real time on all customer channels. Cloud SQL and Cloud Spanner are google cloud solution
    - *Cloud SQL*: Cloud SQL is a fully managed relational database service for MySQL, PostgreSQL, and SQL Server. This frees you from database administration tasks so that you have more time to manage your data. Cloud SQL provides a cloud-based alternative to local MySQL, PostgreSQL, and SQL Server databases. You should use Cloud SQL if you want to spend less time managing your database and more time using it. Many applications running on Compute Engine, App Engine and other services in Google Cloud use Cloud SQL for database storage.
    - *Cloud Spanner*: Cloud Spanner is a fully managed, mission-critical, relational database service that offers transactional consistency at global scale, automatic, synchronous replication for high availability (Copy data across reggion in case of blackout in one region other region provides redundency), and support for two SQL dialects: Google Standard SQL (ANSI 2011 with extensions) and PostgreSQL.

These help organization to maintain Data integrity *i.e, transactional integrity refers to the accuracy and consistency of data stored in a database and scale and roll-back in case of problem like money deducted form account but cash not recieved by atm by the help of transaction history scale* i.e, *scale up and down to meet users demand*.

- *Cloud data warehouse or Data warehouse* : Databases are built and optimized to enable ingesting large amounts of data from many different sources efficiently. However, data warehouses are built to enable rapid analysis of large and multidimensional datasets. 

    Think of the data warehouse as the central hub for all business data. Different types of data can be transformed and consolidated into the warehouse, so they're useful for analysis. In particular, a Cloud data warehouse allows businesses to consolidate data that is structured and semi-structured. Remember that unstructured data tends to be unorganized and qualitative. In other words, it wouldn't fit in a spread sheet. When combined with connector tools, data warehouses can transform unstructured data into semi-structured data that can be used for analysis.

    These are solution by Google Cloud like BigQuery, Pub/Sub, Dataflow
    - *BigQuery*: BigQuery is Google Cloud's fully managed, petabyte-scale, and cost-effective analytics data warehouse that lets you run analytics over vast amounts of data in near real time. Importantly, BigQuery is serverless. This doesn't mean that there's no server. It means that resources such as compute power are automatically provisioned behind the scenes as needed to run your queries. So businesses do not pay for compute power unless they're actually running a query.
    - *Pub/Sub and Dataflow*: Pub/Sub and Dataflow. Pub/Sub is a service for real-time ingestion of data, whereas Dataflow is a service for large scale processing of data. Pub/Sub and Dataflow, can work together to bring unstructured data into the Cloud and transform it into semi-structured data. This transformed data can then be sent directly from Dataflow to BigQuery, where it becomes immediately available for analysis.
    