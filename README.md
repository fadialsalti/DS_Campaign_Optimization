# DS_Campaign_Optimization

Given is the following datatable 'facebook_ad_hourly_v01'. This data contains hourly
breakdown of advertisement data, which ran on Facebooks ad platform. The data
contains the KPIs of multiple campaigns of a business client. Goal of those campaigns is
to increase ticket sales (purchases), as well as too increased visibility (clicks, which result
into homepage views) for promoted events.

Table description:
Campaign_id: id of campaign for one event. One campaign contains multiple ads
ad_id: id of ad running on facebook. Each ad belongs to exactly one campaign.
spend: hourly amount of money spent for this ad
impressions: hourly number of views of this ad on facebook platform
clicks: hourly number of clicks on this ad. A click results into a homepage landing.
purchase: hourly number of purchases made for a event based on this ad.
date: date of ad data sample
time: time of ad data sample

Additional info:
Each ad runs for a certain amount of time. The total runtime per ad can vary between a
few hours and multiple days. The ad data is given in an hourly breakdown.
Problem setup:
- Each campaign starts with a set of different ads. Without prior knowledge, we
are not able to tell which of the ads will perform well or badly in terms of
purchases or clicks.
- In order to have a more efficient campaigns, the goal is to deploy a system which
helps us to identify those well or badly performing ads as early as possible.
Based on this we can switch of ads and keep others running and thus increase
the overall performance of our campaigns. As budget is defined on an ad set
level, switching off ads directs the remaining budgets to running ads and
therefore increases spend on those.

1. Given the data and business goal described above, which algorithms could we,
in theory, use in order to optimize those campaigns in the future? What would
be the advantages and disadvantages of those different approaches with this
given business case & data. Please reason your answers based on the data
given. A basic EDA could help.

2. Lets assume we want to build a prediction model which uses the information of
the first 24 hours of each ad to predict its future performance.
a. Please state two options how you would define a target metric for a
supervised learning approach. Remember that we want to optimize our
system on identifying well performing ads in comparison to poorly
performing ads. State the pros and cons of each definition in terms of
model evaluation, complexity and business goals.
b. Please create and train a prediction model (baseline-model). How do
you evaluate its performance?
c. Based on the results of the previous question and the insights you
created on the data sofar:

How would evaluate the outcome sofar?
Do you think the approach taken will help our business goal and increase overal
campaign performance?
If not so, what are the prohibiting factors for a successful setup? What needs to be
improved?
What other sources of data, or features come into your mind, which could help improve
the models?
Please note that we do not expect exact results or a finally optimized prediction model
here! More important we want to get a good understanding of the decisions taken and
reasons based on the data insight behind them.
