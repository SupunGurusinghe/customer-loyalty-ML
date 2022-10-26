# customer-loyalty-ML
<h2>Introduction</h2>

Retail supermarkets constantly need to know about their customers and shopping behavior. The idea is simply to retain their loyalty and at the same time stretch them to spend more and attract more new customers.

A customer can become loyal only when he/she feel personalized: when they get things from supermarket according to their needs. For example if a customer buys a lot of cereals from a particular brand, upon receiving a discount on his/her next purchase for the very same item, he/she will feel valued for being loyal to the supermarket. More a customer becomes loyal, more deeper the supermarket can dig in his/her shopping behavior so as to keep on deliveing the good customer experience.

In retail, above practice is done by marrying cocnepts like Customer Segmenatation with Personalization. Not only retails; but industries like media, telecommunications, avaiation, financial institutions, insurance, automobiles all over the world are trying to retain this loyalty by focussing their microscopic lens towards the customers shopping behavior. Among them retail industry can do it better just because their data is huge.

<h2>Steps</h2>

<h3>Step 01</h3>
Data Cleaning (Processing) and Creating View:
The given data sets needed some cleaning.

<h3>Step 02</h3>
After cleaning, the three datasets were clubbed together and two views were created:
View number 1: Filtering data to last one year worth of transactions and and calculating annual sales,visits and basket value for a household
View number 2: Creating a Customer Value Model (also called RFM) view from the above view and calculated metrics like Recency, Frequency and Monetary.

<h3>Step 03</h3>
Data Exploration:
high-level understanding about the supermarket by fragmenting sales by type of customers and departments.

<h3>Step 04</h3>
Business Rules (Assumption): While creating the flitered view following business rules were used:
The complete data had five years of data for several products. But for the scope of analysis only one year worth of data was used.
Only those products were included in the Segmentation which were bought by atleast 25 housholds in last one year

<h3>Step 05</h3>
Customer Segmentation:
To deploy Customer VALUE Model, Recency, Freqeuncy and Monetary variables were defined, calculated in Python for each household and added as separate columns. Following definitions were used:
<ul>
<li>Recency: Days since last shop</li>
<li>Frequency: Counts of visits in last 4 weeks</li>
<li>Monetary: Total spend in last 4 weeks</li>
</ul>
Now the K-Mediod clustering algorithm was used to segment customers based on these metrics
