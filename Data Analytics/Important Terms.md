## Data Analytics
- Data analytics is the systematic process of examining raw data to extract meaningful insights, identify patters, and support informed decision making. 
- It uses statistical, mathematical, and computational techniques to transform data into actionable knowledge, often leveraging tools like software, algorithms, and visualisations.

**Two main types of Data Analytics:**
1. **Predictive Analytics**
	- Predictive Analytics is a branch of analytics that makes predictions about future outcomes using historical data combined with statistical modelling, data mining techniques and machine learning.
	- Use cases of Predictive Analysis:
		1. Banks can answer the following questions about their customers
			- Who is likely to default on a loan
			- Which customers pose high or low risks
			- Which customers are most lucrative to target resources and marketing spend
		2. HR teams use predictive analysis and employee survey to:
			- match prospective job applicants
			- reduce employee turnover
			- increase employee engagement

2. **Prescriptive Analytics**
	- It is the practice of analysing data to identify patterns, which can be used to make predictions and determine optimal course of action.
	- Prescriptive Analytics is a sub-discipline within data analytics, itself a practice situated within the disciplines of business analytics and business intelligence. 
	- While predictive is about finding about what might happen next, prescriptive is more about what should we do to make it happen. 

| **Predictive Analysis**                                                                                         | **Prescriptive Analysis**                                                                                        |
| --------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Predicting future outcomes or trends based on historical data.                                                  | Recommending specific actions or decisions to influence outcomes.                                                |
| The scope is narrow as it focuses on estimation, probabilities, and forecasting without direct action guidance. | The scope is broad as it extends predictions to include scenario evaluation, optimisation, and decision support. |
| Relies on statistical modelling, machine learning, and data patterns                                            | Builds on predictive models with optimization techniques, simulations, and rules                                 |

---

## Business Optimisation
Business optimisation is the process of enhancing an organisation's business operations, workflows and strategies to achieve maximum efficiency and align with their long-term objectives. 

It involves actions including but not limited to, streamlining business processes, improving resource allocation, and leveraging tools such as automatic and data-driven insights to reduce costs and boost performance. 

**Key characteristics of Business Optimisation**
1. Business Process Management - Standardising processes to ensure consistency and efficiency across departments.
2. Process Improvement - Continuously refining workflows to eliminate waste and improve productivity
3. Real-Time Monitoring - Using real-time data to track performance and respond quickly to disruptions or opportunities
4. Eliminating Bottlenecks - Identifying and resolving inefficiencies that slow down operations.

---

## The 5 Vs of Big Data

> Big data refers to extremely large and complex datasets that traditional processing tools can't handle efficiently. It involves collecting, storing, analysing, and extracting value from massive volumes of data generated from various sources like social media, sensors, transactions, and more.

The 5Vs of big data consists of:
1. Data Volume
2. Data Velocity
3. Data Variety
4. Data Veracity
5. Data Value

#### Data Volume
- Data volume refers to the sheer amount of data being generated, processed and stored every second from countless sources.
- In this era of big data, we are talking about handling hundreds of gigabytes, petabytes and  even exabytes of data.
- Traditional databases and servers cannot handle this kind of data volume and leads to data loss, overload, and processing bottlenecks.

#### Data Velocity
- Data velocity describes the speed at which data is generated, streamed, must be processed. Along with extremely fast generation speed, we also need systems that can keep up with that rate.
- It is required as delayed responses in a time crucial environment such as stock market can lead to financial loss.
- Businesses must invest in systems which can handle data in motion to enable timely decisions.

#### Data Variety
- Data variety refers to the diverse types, formats and structures of data. It can be either structured (spreadsheets, tables, etc.), semi structured (JSON, etc.) or raw (e.g.: images, audios, videos, etc.)
- Integrating these many different types of data into something meaningful and informative is really difficult leading to flawed analysis and errors.

#### Data Veracity
- Data veracity basically refers to the reliability, accuracy, consistency, and trustworthiness of data. 
- It encompasses issues like errors, biases, incompleteness or misinformation and ensures that the data is true enough to base decisions on, rather than being corrupted or uncertain.
- Flawed information leads to Garbage In, Garbage Out situation. It also leads to faulty predictions or misguided strategies. 

#### Data Value
- Data value refers to the usefulness, relevance, and potential economic or strategic benefit of data to an organisation.
- It's about the quality of data in solving specific problems, providing competitive advantage over others, or driving revenue.
- Value is subjective; Data that is gold to one organisation might be trash to the another.

---

## Data Warehouse, Data Lake, Data Mart

#### Data Warehouse
- A data warehouse is a centralised and structured system that collects and stores vast amounts of historical data from various sources to support business intelligence.
- It is designed for storing, managing, and analysing large volumes of historical, integrated data from multiple sources.
- Key features:
	1. Subject Oriented - A data warehouse provides information on a topic rather than ongoing operations of the organizations.
	2. Integrated - Establishing standard unit of measurement from the different databases for all the similar data.
	3. Time Variant - The data collected in a data warehouse is acknowledged over a given period of time and provides historical information. Therefore, each record must contain an element of time.
	4. Non-Volatile - All the data in a warehouse is non-volatile meaning that the prior data will not be erased.

#### Data Lake
- A data lake is similar to a data warehouse but here the data can be structured, unstructured, or even in raw format.
- It is a scalable, centralised for raw, unprocessed data in its raw format.
- Key featuers:
	1. "Schema on read" approach: Data is stored as it is and structured only when needed
	2. Handles big data volumes and variety.

#### Data Mart
- A data mart is a focused subset of data warehouse designed to serve the analytical needs of a specific department, business unit, or teams, such as finance or marketing.
- It's essentially a "mini data warehouse" for targeted analysis.
- Key features:
	1. Contains pre-aggregated, summarised data relevant to one domain. (e.g.: marketing or finance)
	2. Can be independent or independent
	3. Faster to implement that full warehouse.

---

## OLTP
**OLTP (Online Transaction Processing)** is a type of database management system designed for handling high volumes of short, real-time transactions efficiently.

> It's prime focus is on processing operational data such as inserts, updates, deletes, and simple queries quickly and reliably, ensuring data integrity and [^1]**atomicity**. 

**Key characteristics of OLTP**
1. High Transaction Rate: Supports thousands of concurrent operations per second, with low latency (e.g.: milliseconds for ATM withdraws or e-commerce checkout)
2. Normalised Data Structure: Uses relational database with normalised schemas to minimise redundancy and prevent anomalies during frequent updates.
3. Focus on Current Data: Deals with latest operational data; not optimized for historical data analysis.
4. Consistency and Reliability: Emphasizes error-free processing, often with rollback capabilities for failed transactions.

---

## OLAP
OLAP (Online Analytical Processing) is a technology and framework for analyzing multidimensional data from multiple perspectives, enabling complex queries, and business intelligence tasks.

Unlike OLTP, which handles real-time transactions, OLAP is designed for decision support, focusing on historical and aggregated data to uncover:
- Trends
- Patterns
- Insights

> OLAP powers data warehouses, data marts and analytical tools, making it essential for strategic planning in big data environments. 

**Key characteristics of OLAP**
1. Multidimensional Analysis: Organizes data into dimensions (e.g.: time, geography, product) and measures (e.g.: sales revenue), allowing interactive exploration without restructuring the database.
2. Historical and Denormalized Data: Works with integrated, often denormalized data from multiple sources; focuses on "what happened and why" rather than current operational updates.
3. Complex Queries and Aggregation: Supports operations like summarizing, rotating views, and slicing (focusing on subsets). Optimized for read-heavy, infrequent but intensive queries.

---

## Data Mining
Data mining is the overall process of identifying patterns and extracting useful insights from big data sets, using machine learning and statistical analysis to uncover patterns and other valuable information from large data sets.

**Key Purposes of Data Mining**
1. **Descriptive**: Summarizing data through observations of patterns, associations, correlations, clustering, and outlier identification.
2. **Predictive**: Forecast outcomes using ML models for trends or real-time responses.




[^1]: **atomicity** refers to the principle that a transaction must be treated as a single, indivisible unit meaning that it either completes (all changes are applied) or fails completely (no changes are applied). This ensures data integrity by preventing partial 

