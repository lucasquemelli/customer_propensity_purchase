# Customer Propensity to Purchase

<code><img width="100%" src="https://github.com/lucasquemelli/customer_propensity_purchase/blob/main/Images/propensity_purchase.png"></code>

# 1. Business Problem

Description

---

Our Client is an early-stage e-commerce company selling various products from daily essentials (such as Dairy & vegetables) to high-end electronics and home appliances. It is a one-year-old company and they are witnessing many people coming to their platform and searching for products but only a few end up purchasing.

To increase the number of purchases, the business is planning to send discounts or coupons to users to motivate them to buy. But since it is an early-stage startup, they have only limited funds for this discount campaign. So, they have reached out to us seeking our help in building a model that would predict the purchase probability of each user in buying a product.

We will be making use of propensity modeling for this. Propensity modeling is a set of approaches to building predictive models to forecast the behavior of a target audience by analyzing their past behaviors. That is to say, propensity models help identify the likelihood of someone performing a certain action. We can then use this likelihood or probability score to create personalized targeting campaigns for the users thus reducing our total cost (targeting only a small set of users) and increasing our ROI.

To help us in predicting the propensity of purchase, we will also make use of RFM Modeling. RFM is a data-driven customer segmentation technique that allows marketers to make informed decisions. RFM stands for Recency, Frequency, and Monetary value, each corresponding to some key customer trait. These RFM metrics are important indicators of a customer’s behavior because the frequency and monetary value affect a customer’s lifetime value, and recency affects retention, a measure of engagement.

It empowers marketers to quickly identify and segment users into homogeneous groups and target them with differentiated and personalized marketing strategies. This in turn improves user engagement and retention. With the probability scores from propensity modeling, the marketing team can filter only those users who need the actual push (in terms of discounts or coupons) to make a purchase rather than sending coupons to users who would have bought the product anyway.

**Purpose:** To build a model to predict the purchase probability of each user in buying a product for an e-commerce company with the help of the propensity model.

**Strategy:** we used the CRISP-DS (Cross-Industry Process - Data Science) as the main project management methodology.

# 2. Business Assumptions (Formulated Hypotheses)

The following hypotheses (questions in this case) were formulated in order to be tested/answered:

**1.** How many unique users in the data and how many of them purchased at least once? Also, what is the average number of purchase per customer?

**2.** Which is the most purchased category and sub-category?

**3.** Do people add the products to cart before they purchase or buy directly?

**4.** What is the average and median time taken by a user to buy a product?

**5.** What is the average and median time between repeated purchases?

**6.** What is the trend of unique users across time period?

**7.** What is the trend of purchase across the time period?

# 3. Solution Strategy

**Step 01 - Data Description:** cleaning data, changing data type, treating missing values and descriptive statistics.

**Step 02 - Feature Engineering:** creating new features that may better explain the phenomenon.

**Step 03 - Feature Filtering and Selection:** rows filtering and columns selection.

**Step 04 - Balanced Dataset:** balance of the dataset.

**Step 05 - Exploratory Data Analysis (EDA):** univariate analysis, bivariate analysis (hypotheses test) and multivariate analysis.

**Step 06 - Data Preprocessing:** rescaling, encoding and transformation.

**Step 07 - Feature Selection:** removing high correlated features and using Boruta algorihtm with Random Forest Regressor to select the most relevant features.

**Step 08 - Machine Learning Modelling:** testing and comparing Machine Learning models.

# 4. Top 2 Data Insights

**2.** Which is the most purchased category and sub-category?

**Category:** mobile and accessories. 

**Subcategory:** tops. 

**3.** Do people add the products to cart before they purchase or buy directly?

**Total unique users who purchased:** 167.

**Total direct buy (without adding to cart):** 20.

**Total add_to_cart buy:** 147.

# 5. Business Results

Random Forest and Logistic Regression predicted propensity to purchase of a user with 100% of average accuracy. However, we have a small dataset, then our model probably overfits.

6. Conclusions

We used Artifical Neural Network (ANN) to predict users propensity to purchase, yet due to the low number of rows, this model did not perform well. Thus, we used Random Forest Regression and Logistic Regression and we achieved an average accuracy of 100%. Yet, we must remember that we have a small dataset, which means our model probably overfits.

# 7. Next Steps

In an ideal problem solution, we should collect much more data in order to take conclusions and finish properly our project. Thus, we suggest this step in order to improve our project. 
