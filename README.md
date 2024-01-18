# **Potential-Customer-Prediction**

## **Context**
The EdTech industry has been surging in the past decade immensely, and according to a forecast, the Online Education market would be worth $286.62bn by 2023 with a compound annual growth rate (CAGR) of 10.26% from 2018 to 2023. The modern era of online education has enforced a lot in its growth and expansion beyond any limit. Due to having many dominant features like ease of information sharing, personalized learning experience, transparency of assessment, etc, it is now preferable to traditional education.

In the present scenario due to the Covid-19, the online education sector has witnessed rapid growth and is attracting a lot of new customers. Due to this rapid growth, many new companies have emerged in this industry. With the availability and ease of use of digital marketing resources, companies can reach out to a wider audience with their offerings. The customers who show interest in these offerings are termed as leads. There are various sources of obtaining leads for Edtech companies, like

The customer interacts with the marketing front on social media or other online platforms.
The customer browses the website/app and downloads the brochure
The customer connects through emails for more information.
The company then nurtures these leads and tries to convert them to paid customers. For this, the representative from the organization connects with the lead on call or through email to share further details.

## **Objective**
ExtraaLearn is an initial stage startup that offers programs on cutting-edge technologies to students and professionals to help them upskill/reskill. With a large number of leads being generated on a regular basis, one of the issues faced by ExtraaLearn is to identify which of the leads are more likely to convert so that they can allocate resources accordingly. You, as a data scientist at ExtraaLearn, have been provided the leads data to:

Analyze and build an ML model to help identify which leads are more likely to convert to paid customers,
Find the factors driving the lead conversion process
Create a profile of the leads which are likely to convert

## **Exploratory Data Analysis**

* Performed Data Cleaning and checked statistical summary
* Extensive Univariate and Bivarite Analysis
* Outlier Detection
* Checking distribution of each features

*Related Images :*

![bivariate_1](https://github.com/moinul-hossain-dhrubo/Potential-Customer-Prediction/assets/122023969/8598a66e-18d3-471d-ad68-cc0e2e934e6d)
![corr_mat](https://github.com/moinul-hossain-dhrubo/Potential-Customer-Prediction/assets/122023969/db04872c-71a4-4f4a-b42e-1cf8b9e18bc5)

## **Machine Learning Model Training**

* Utilized Decision Tree and Random forest classifier
* Tree pruning technique was used to reduce overfitting
* Hyperparameter Tuning with RandomizedSearchCV and GridSearchCV
* Finding feature importance

*Related Images :*

![max_depth_vs_error](https://github.com/moinul-hossain-dhrubo/Potential-Customer-Prediction/assets/122023969/1cedff48-cc55-4738-8af7-5328149eafe9)
![random_forest_tree](https://github.com/moinul-hossain-dhrubo/Potential-Customer-Prediction/assets/122023969/17b63285-a883-424f-9d54-ce23a0697e65)
![result_rf](https://github.com/moinul-hossain-dhrubo/Potential-Customer-Prediction/assets/122023969/39b44cfc-0113-4e26-b914-df472776714d)

## **Actionable Insights**

* We were able to create a lead conversion prediction model with Random Forest that had a decent overall performance and an ~88% recall rate.

* Based on feature importance from classification and EDA, several factors seem to be influencing conversion:

1. Time spent on the website
2. Having one's first interaction through the website
3. Profile completeness at or above medium

* Followed by:
4. Professional activity (non-student)
5. Age (toward late career)
6. Last activity was through the website

* Also:
7. Referrals could be playing a role into the conversion decision.

Based on these, late-career professionals who are working or unemployed, who have spent substantial time on the website, possibly finishing their profile, are the leads most likely to convert.

However, EDA has identified the following issues:
* The model does not do a satisfactory job of capturing the impact of advertising channels.
* Additionally, the data does not discuss any potential associations or the combined effects of several advertising sources.
* Leads who joined without browsing the website have lower conversion rates than those who did.
* Lead conversion rates are much lower for leads who first engaged with the mobile application.
* There aren't any details in the data on how time is spent on the website.

## **Business Recommendations**

* Website Interaction:
The business should concentrate on website interactions. Perhaps the website's front-end and back-end developers can have a significant impact by making it more persuasive and appealing.

* App Developement:
The app may not be user-friendly, users may not be interested in downloading it, or we may be missing out on something. It need more research.

* Lead Behaviour:
Knowing what the leads are actually doing on the website will be useful information. That will make things clearer.

* Promotional Offers:
Due to the fact that students appear to have the lowest conversion rates, the organization can offer special discounts to them. e.g. The business can deliver tailored messages if it recognizes a customer as a student. Offers that are open to everyone may help improve conversion rates.

* Advertise Analysis:
The information given does not make it obvious how advertising channels affect consumers. We can only conclude from the analysis that referral incentives should be considered. e.g. referral code discounts.

* Incentivize profile completion:
Increased completion might be achieved by redesigning the questionnaire or adding a reward for finishing the profile.

* Decide on recall value/budget :
If the company proposes a fixed recall value according to their budget, then we can focus on precision with a fixed recall value for different models.