# **Will the Customer Accept the Coupon?**

### **Project goal:** 

This assignment is to find out whether a customer will accept a restaurent coupon delivered to their phone while driving near the location. Perform an Exploratory Data ANalysis (EDA) to answer the question.

### **Problem Context:** 

Would you accept that coupon and take a short detour to the restaurant? Would you accept the coupon but use it on a subsequent trip? Would you ignore the coupon entirely? What if the coupon was for a bar instead of a restaurant? What about a coffee house? Would you accept a bar coupon with a minor passenger in the car? What about if it was just you and your partner in the car? Would weather impact the rate of acceptance? What about the time of day? 

What are the factors that determine whether a driver accepts the coupon once it is delivered to them? How would you determine whether a driver is likely to accept a coupon?

## **Notebook & Data**

 The Jupyter Notebook containing the analysis of the problem can be found here: [Notebook](https://github.com/sreela-gopi/Practical_Application_5_1/blob/main/practical_assignment_5_1_prompt.ipynb) <br>
 The dataset provided for the analysis can be found here : [Dataset](https://github.com/sreela-gopi/Practical_Application_5_1/blob/main/data/coupons.csv)

## **Findings of the analysis**
Across the five different types of coupons - less expensive restaurents (under 20), coffee houses, carry out & take away, bar, and more expensive restaurents(20 - $50), **around 57% of the people accepted the coupons**.

*   **Type of coupon matters**

   1. Number of Coffee House coupons are distributed and accepted the highest.
   2. Number of More expensive Restaurent coupons are distributed the lowest.
   3. Coupon acceptance proportion is higher for less expensive restaurents and Carry out & Takeaway
   4. Coupon rejection proportion is higher for Bar and More expensive restaurents
*   **Temperature of the day has an impact**   
  1. More number of Coupons are delivered when temperature is higher
  2. There is no clear pattern in the distribution of temperature across the data
  3. Drivers are more likely to accept the coupons as temperature goes higher

### **Bar coupon insights:** 

  Around 41% of the Bar coupons were accepted.
*  **The number of times the drivers visit a bar in a month is an indicator**    
  1. Coupon acceptance rate is higher for the category of drivers who went to the bar 3 or fewer times a month than who went more.
  2. Among the drivers who went to bars more than once a month and had passengers that were not a kid, those who were NOT widowed are tend to accept the Bar coupons more than who were widowed.
  3. Drivers who went to bars more than once a month and had passengers that were not a kid and were widowed do not seem to accept the Bar coupons
*   **Age of the driver is a factor** 
  1. Drivers who went to bar more than once a month are tend to accept the Bar coupons more when they are over the age of 25 than under age people
  2. Drivers who went to bar less than once a month are tend to accept the Bar coupons more when they are over the age of 25 than under age people
  3. Among the drivers who are over the age of 25, those who went to bar less than once a month are tend to accept the Bar coupons more than those who visited bar more
  4. Drivers who went to bars more than once a month are more likely to accept the Bar coupons when they are under the age of 30, than over 30

*   **Occupation has an role** 
  1. Drivers who had occupations in farming, fishing, or forestry who go to bars more than once a month do not accept the coupons irrespective of them having kids as passengers.
  2. Drivers who had occupations in farming, fishing, or forestry who go to bars less than once a month are very unlikely to accept the coupons irrespective of them having kids as passengers.
  3. Among the drivers who had occupations other than farming, fishing, or forestry and had passengers that are kids, those who went to bars less than once a month are tend to accept the Bar coupons more than who visited bars more.
  4. Among the drivers who had occupations other than farming, fishing, or forestry and had passengers that are not a kid, those who went to bars less than once a month are tend to accept the Bar coupons more than who visited bars more.

### **Coffee House coupon insights:**

  Around 50% of the Coffee House coupons were accepted.
*   **Time of the day matters** 
 1. Starting from morning, the acceptance rate of Coffee House coupons increases.
 2. During the morning hours around 10am is the highest number of Coffee House coupon acceptance rate.
 3. In the Afternoon hours the acceptance rate slighly decreases.
 4. At night around 10 pm the coupon acceptance is very low.
*   **The number of times  adriver visits coffee house in a month plays a role**  
 1. Among the people who go to a coffee house people who go 1 to 3 times a month has the highest rate of acceptance.
 2. People who never visit coffee house has the lowest rate of acceptance.
 3. People who visit more number of times a month has lower acceptance rate than who visits less.
 4. Among all age groups, people who went to coffee house 1-3 times a month are tend to accept the coupon.
 5. Among all age groups, people who never went to coffee house in a month are tend to reject the coupon.
*   **Age is a factor**  
 1. Drivers in the age range below 21 has the highest rate of acceptance of Coffee House coupons
 2. Drivers in the age rage 30 and 35 are tend to reject the coupons.
 3. Acceptance ratio decreases with as age increases.
*   **Destination of the driver decides** 
 1. Drivers whose destination is No Urgent Place are tend to accept the coupons.
 2. Drivers who are going home or work are tend to reject the coupons.
*   There is no good correlation exists between the numerical features in deciding the Coffee House Coupon Acceptance
*   A very weak positive correlation is seen between temperature and Acceptance
*   A very weak negative correlation is seen between age and Acceptance

## **Actionable insights & Business Recommendations**
1.   Age is an important feature that affects the acceptance of bar coupon which is easy to track. So delivering bar coupons to appropriate age group will do good for the business
2.   Unemployed people has the highest rejectio rate. So, delivering the bar coupons based on a basic varification as employed or unemployed will be good for business.
3. Destination of a driver is an important factor that affects the coupon acceptance rate. So delivering coffee house coupons based on the possible destination can do good for business.
4. Delivering the coupon, based on the time of the day can be good for business as time as a good impoact in acceptance rate.


## **Next steps & Future Recommentions**
1. The dataset contains columns that are not relevant in deciding the accepatnce rate of the coupons like `car` which contains many missing values. Irrelevant data could be avoided to have precise analysis.
2. Confusing data columns are present like `toCoupon_GEQ5min`, `toCoupon_GEQ15min`, `toCoupon_GEQ25min` whose values are difficult to interpret. This affects the quality of the analysis. If these are not important, they could be avoided.

## **Tech Stack**

**Python:** Pandas, NumPy <br>
**Data Visualization:** Matplotlib, Seaborn

This assignment was completed as part of the Practical Assignment 5.1 of  Professional Certificate in Machine Learning & Artificial Intelligence - March 2025



