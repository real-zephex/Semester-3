**Ques 1**
Is it correct to say that “data is objective, but information is subjective”? Discuss with examples, considering the distinction between Data, Facts, and Information.

**Solution**
Data is indeed objective in the sense that it consists of raw, unprocessed facts, and figures, often collected through measurements, surveys, observations and other forms of data collection. Data on its own does not provide much context and understanding of what it is trying to represent.
The data is objective because it presents facts without any interpretation.

Now, if that same data is processed, analyzed, and interpreted then it takes the shape of `information`. An information is a piece of data from which we can derive some meaning and gain understanding about what that data is trying to represent.

For example:
Every hospital keeps record of all its visitors, all of this data is stored in a database which might contain the following attributes:
- Patient names
- Ages
- Medical conditions (e.g.: diabetes, hypertension)
- Treatment plans (e.g.: medication, surgery)
- Lab test results (e.g.: blood pressure, blood glucose results)

Now, raw data like above, consists of numbers, dates, and text. Without interpretation, it's difficult to understand the significance of the information. 

If we process this data and derive meaningful interpretations such as follows then it becomes information:
1. List of all patients who have been diagnosed with same disease in last 2 months.
2. List of all patients who are at "high risk" for complications for a particular condition.
3. A hospital administrator reports that the hospital's patients' satisfaction ratings are improving or declining.

Having the above insights at hand will give us a much better understanding of what we are dealing with and will assist us in informed decision making.

To fully address the statement "data is objective, but information is subjective", we need to to examine why information introduces an element of subjectivity, even as it builds on objective data. While data remains neutral and uninterpreted, the process of converting it into information introduces an element of of human judgement, context, and perspective--which all varies from person to person. This is where subjectivity is introduced: the same raw data might be interpreted differently based on the analyst's expertise, biases, goals, or available context, leading to different "meanings" or "decisions".

In the above example, consider a raw data point like blood sugar levels of a patient of 200 mg/dL. This is objective data---just a measured fact. But when processed into information, 
1. A doctor might interpret it as "high risk for diabetic complications" based on medical guidelines and the patient's age.
2. A hospital administrator might view the same data as part of a trend showing "rising average glucose levels across diabetic patients," suggesting a need for better preventive care programs.
3. A researcher could interpret it subjectively as evidence of "environmental factors like diet in urban areas contributing to poor control."

Now, let's talk about distinctions between Data, Facts, and Information:

1. **Data**
	- It refers to raw, unprocessed, and often unstructured facts and figures collected from various sources.
	- Data can be in the form of numbers, text, images, or sounds.
	- Data on its own does not provide any meaningful insights or context.

2. **Information**
	- Information is that data that has been processed, organized, and structured to provide meaning and context.
	- Information helps to answer questions, solve problems, or make informed decisions.

3. **Facts**
	- Facts are verified and confirmed pieces of information that are objective and unbiased.
	- Facts are often considered to be absolute and unchanging.
	- Facts can be used to support or contradict information.

---

**Ques 2**
Challenges of data creation are explained in terms of Volume, Velocity, and Variety. How can this be extended to include Veracity and Value? Discuss with examples.

**Solution**
The 3Vs of Big Data --- Data Volume, Data Velocity, and Data Variety are foundational challenges in modern data creation and management.

**Data Volume - The How Much problem**
- Data volume refers to the sheer amount of data being generated, processed, and stored every second from countless sources like IoT devices, sensors, social media platforms, etc.
- In this era of big data, we are talking about handling gigabytes, terabytes, and petabytes of data.
- Traditional computers and servers are unable to handle this level of traffic and often lead to system crashes, data corruption, data overload and other several issues. This creates a need for scalable infrastructure like cloud storage which help in preventing data silos which lead to data becoming inaccessible or unstable.

**Data Velocity - The How Fast problem**
- Data velocity refers to the speed at which the data is being generated, streamed and must be processed. Along with systems generating data at high speeds, we also need systems which can process this data at high speed.
- In a fast paced world, any delay can lead to financial losses (e.g.: stock market, 2010 Flap Crash) or security risks (e.g.: fraud detection).
- Businesses need solutions which can handle data in motion to enable timely decisions.

**Data Variety - The How Diverse problem**
- Data variety refers to the diverse types, formats, and structure of data. It can be either structured (spreadsheets, tables, etc), semi-structured (JSON, XML, etc.), or unorganized (videos, images, audios, texts, etc.)
- Integrating all these different formats and deriving something useful is difficult due to flawed analysis and errors.

 **Data Veracity - The How Accurate problem**
 - Data veracity refers to the accuracy, reliability, consistency, and trustworthiness of data. 
 - Veracity is about ensuring that the data is true enough to base decisions on, rather than being corrupted.
 - Flawed information leads to Garbage In, Garbage Out situation. It also leads to faulty prediction or misguided strategies.

**Data Value - The How Important problem**
- Data value refers to the usefulness, relevance, and potential economic or strategic benefit of data to an organization.
- It's about quality of data in solving specific problems, providing competitive advantage over others, or driving revenue.
- Value is subjective; data that is gold to one company might be worthless to other.

**Example**
###### Amazon's Black Friday E-Commerce Analytics (2019 Peak Sales Event)
During Amazon's Black Friday/Cyber Monday in 2019, the platform handled an unprecedented surge in online shopping, processing over 175 million items sold globally in a single weekend.

- **Volume**: Enormous scale—Amazon processed petabytes of data, including billions of page views, search queries, and purchase records. For instance, over 100 million unique visitors generated logs of clicks, carts, and transactions, overwhelming traditional databases and requiring distributed storage like S3 to avoid crashes.

- **Velocity**: Data streamed in at lightning speed—up to 1.5 million orders per hour during peak hours, with live updates on stock levels and recommendations. This high speed demanded real-time processing to prevent stockouts (e.g., popular items like electronics selling out in minutes), using stream analytics to adjust prices dynamically.

- **Variety**: Data came in all forms: structured (e.g., transaction IDs and prices), semi-structured (e.g., user reviews in JSON), and unstructured (e.g., product images, voice searches via Alexa, or social media shares). Integrating this from global sources (e.g., mobile apps in different languages) was tricky, requiring AI for image recognition and NLP to handle diverse inputs like emojis in reviews.

- **Veracity**: Quality issues abounded—fake reviews (e.g., bot-generated 5-star ratings inflating product popularity), location data errors from VPN users, or inconsistent inventory counts due to warehouse delays. Amazon estimated 10-20% of data noise from fraud, so they used machine learning for anomaly detection and verification against trusted sources to maintain accuracy.

- **Value**: The payoff was huge: insights like "trending categories in real-time" allowed personalized recommendations, boosting sales by 20-30% (per industry reports). For example, analyzing velocity and variety data revealed regional trends (e.g., more toy demand in the US vs. electronics in Asia), enabling targeted promotions that generated billions in revenue.