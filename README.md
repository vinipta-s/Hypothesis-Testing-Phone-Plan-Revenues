# Hypothesis Testing Phone Plan Revenues
Summary: In this project, a preliminary analysis of two plans offered by Megaline was done on a small client selection (500 Megaline clients) to determine which of the plans brings in more revenue in order to adjust the advertising budget. The data sets were explored, cleaned and merged. Data was visualized for understanding customer behavior in using the services and revenue distribution for the two plans.

Prompt: The telecom operator Megaline offers its clients two prepaid plans, Surf and Ultimate. The commercial department wants to know which of the plans brings in more revenue in order to adjust the advertising budget. This is a preliminary analysis of the plans based on a relatively small client selection (500 Megaline clients)

The data for 2018:
* megaline_plans.csv — plans, what is included in each and the cost of exceeding those included services.
* megaline_users.csv — 500 users, their info and plan, start and end dates
* megaline_calls.csv — calls and duration of calls
* megaline_internet.csv — mb used for each session
* megaline_messages.csv — messages sent

**Goal: Determine which plan brings in more monthly revenue and look into the behavior of the clients for messages, calls and internet use.**

Summary of Project by sections:
1. Initialize Libraries
2. Datasets were loaded and sampled, and checked for missing values and duplicates. Data was cleaned and a new dataset consisting of the sum of services per user per month was created and merged with other datasets on user_id.
3. Monthly revenue was calculated for each user per month and the services that exceeded the limit of their plans. 
4. Looked at user behaviors by ploting their monthy usage and revenue distribution.
5. Statistical test hypothesis: the equal_var parameter set to False to account for any variance as a result of the imbalance data size. Used bootstrap mean confidence intervals for determining which plan produces a higher monthly revenue.
6. <b>Final Report: </b>
