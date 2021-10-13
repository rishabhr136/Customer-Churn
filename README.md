# Customer-Churn: "Predict behavior to retain customers. You can analyze all relevant customer data and develop focused customer retention programs."
Each row represents a customer, each column contains customer’s attributes described on the column Metadata.  The data set includes information about:  Customers who left within the last month – the column is called Churn Services that each customer has signed up for – phone, multiple lines, internet, online security, online backup, device protection, tech support, and streaming TV and movies Customer account information – how long they’ve been a customer, contract, payment method, paperless billing, monthly charges, and total charges Demographic info about customers – gender, age range, and if they have partners and dependent
The business objective is to predict the churn in the last (i.e. the ninth) month using the data (features) from the first three months. To do this task well, understanding the typical customer behaviour during churn will be helpful.
Understanding Customer Behaviour During Churn Customers usually do not decide to switch to another competitor instantly, but rather over a period of time (this is especially applicable to high-value customers). In churn prediction, we assume that there are three phases of customer lifecycle :
The ‘good’ phase: In this phase, the customer is happy with the service and behaves as usual.
The ‘action’ phase: The customer experience starts to sore in this phase, for e.g. he/she gets a compelling offer from a competitor, faces unjust charges, becomes unhappy with service quality etc. In this phase, the customer usually shows different behaviour than the ‘good’ months. Also, it is crucial to identify high-churn-risk customers in this phase, since some corrective actions can be taken at this point (such as matching the competitor’s offer/improving the service quality etc.)
The ‘churn’ phase: In this phase, the customer is said to have churned. You define churn based on this phase. Also, it is important to note that at the time of prediction (i.e. the action months), this data is not available to you for prediction. Thus, after tagging churn as 1/0 based on this phase, you discard all data corresponding to this phase.
In this case, since you are working over a four-month window, the first two months are the ‘good’ phase, the third month is the ‘action’ phase, while the fourth month is the ‘churn’ phase.


Observations Based on Visualizations
Observation-1: Whether male or female, if they do not have partner or dependents, they are more likely to churn!!¶
Observation-2: During 0-10 years of tenure, we can see maximum churning. As the customer turns old, they might get habituated using same telecom service
Observations-3: People with Phone services (yes) and 'Fiber optic' Internet Service are churning more
Observations-4:more churning takes place in first 10 yrs, for customers with or without tech support. But Churning is more in case of "without tech support" customers
Observations-5: As the monthy charges are incresing, we can see the density increasing too (60-120), which means more churning with increasing monthly charges
Observation-6: It is quite opposite of what has been seen for monthly charges. Here high churning occurs in early phase itself, 0-2000 total charges have maximum churning
Observation-7: Churning is being observed equally for the 'Yes', 'No' group of whether connected StreamingTv or not!
Observation-8: Churning is being observed equally for both the 'Yes', 'No' group of StreamingMovies
Observations-9: clearly visible that customers with month-to-month contract are the highest churners
Observation-10: Most churners are non-senior citizens. Although we should also consider the fact that, data is more for non-senior citizens (5:1)
![download](https://user-images.githubusercontent.com/68055586/137069256-15316626-0320-4249-867a-878a15484520.png)
