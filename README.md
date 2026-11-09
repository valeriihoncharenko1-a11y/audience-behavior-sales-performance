**Goal**: 
The objective of this project was to analyze user behavior and sales performance to identify patterns in revenue dynamics, user conversion, and purchasing activity across devices and traffic channels. The analysis aimed to evaluate the registration-to-purchase funnel, explore differences between user segments, and identify potential opportunities for improving conversion and revenue performance.


**Conclusions**:


***Product Analytics***:

*Core Revenue Drivers*: 
Sofas & armchairs, Chairs, Beds, Bookcases & shelving units and Cabinets & cupboards form class A and generate about 80% of revenue. Sofas and Chairs lead in both sales volume and revenue. Bookcases lead in volume but are lower in revenue because of a low price, while Beds contribute to revenue through high-ticket sales.

*Assortment Optimization*: 
By revenue, Bar furniture and Children’s furniture fall into class C. Children’s furniture has mid-table sales volume but low revenue due to low prices. Along with Nursery furniture, Café furniture, Sideboards and Room dividers, these categories together contribute only a small share of revenue.It is recommended to review their marketing strategy or optimize production.


***Marketing & Geography***:

*Traffic & Revenue Relationship*: 
The analysis identified several patterns in sales performance and user behavior. Weekly revenue generally followed sales volume, with a peak in early December followed by a decline, suggesting that traffic volume may be an important driver of revenue fluctuations. Desktop generated a substantial volume of purchasing sessions, while Organic Search and Paid Search accounted for the largest shares among the displayed traffic channels. However, these volume metrics alone do not establish which devices or channels perform most efficiently.

*Regional Optimization & Markets*: 
The United States is the dominant market, generating both the highest number of shopper sessions and the largest share of total revenue, falling into Category A. India and Canada are the next-largest markets, though at a fraction of US volume.

*Conversion Funnel*: 
The conversion rate from registered users to paying users was approximately 9.95%, highlighting the registration-to-purchase journey as a key area for further investigation.


***Tech Insights***:

*Statistical Insights*: The statistical tests identified no statistically significant differences in order value across countries, browsers, subscriptions, devices, or traffic channels, whereas session volume and revenue demonstrate a statistically significant correlation, and daily sales show a statistically significant difference across traffic channels.



**Link to dashboard**:
https://public.tableau.com/views/AudienceBehaviorSalesPerformance/Dashboard1?:language=en-US&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link



**Notes**:
For Revenue was used price column because of the lack of more convenient data.
Dataset contains only three months of recorded data, so it’s impossible to say whether tendencies are seasonal or general.

**Dataset Description**:
This dataset describes the behaviour of online shop visitors at the level of individual sessions. It contains detailed data on every visit to the site — from device specifications and traffic sources to the actions of logged-in users and their purchases.
As this is a pivot table, each row corresponds to a single session. The data covers the period from 1 November 2020 to 31 January 2021.

Null values in "language", "continent" and "country columns"(although in last two it was filled as "(not_set)") occurred because users did not fill them in, or due to problems with scraping data from the original website. In columns "registered_user_id", "is_verified", "is_unsusribed" blank values was left for users that doesn't refistered. And if for "product_category", "product_name", "price" and "short_description" missing values there occuring when there was no purchse within the session.

session_date:the date of the user’s session.

ga_session_id: a unique session identifier.

continent: the continent from which the visit originated.

country: the user’s country of residence.

device: the type of device used by the visitor.

browser: the user’s web browser.

mobile_model_name: the model of the mobile device.

operating_system: the device’s operating system.

language: the language of the user’s browser or device interface.

traffic_source_info: information about the traffic source.

traffic_channel: generalised traffic acquisition channel.

registered_user_id: unique user identifier.

is_verified: account verification flag (1 — account verified, 0 — not verified).

is_unsubscribed — flag indicating whether the user has unsubscribed from newsletters or the service (1 — unsubscribed, 0 — active subscriber).

product_category: category of the purchased product.

product_name: the name of the specific product purchased.

price: price of the purchased product.



**Tech Stack**:

SQL (BigQuery) – data extraction.

Python (Pandas, NumPy, SciPy, Statsmodels, Matplotlib, Seaborn) – data analysis and statistical testing.

Tableau – data visualization.



**Project Workflow**:

Data extraction using SQL and BigQuery.

Data exploration and quality assessment.

KPI calculation (CR, ARPU, ARPPU).

Exploratory data analysis.

Statistical hypothesis testing.

ABC analysis.

Dashboard creation and business recommendations.

 
