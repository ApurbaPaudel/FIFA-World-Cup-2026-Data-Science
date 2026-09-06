ANALYTIC TASK 2

Among players at the FIFA World Cup 2026, do younger players(aged 23 or younger) commit significantly more fouls per 90 minutes than older players(aged over 23)?

Data Wrangling
Source: FBref.com - Miscellaneous Stats
Cleaning steps:
Checked to parse the age format into a decimal age.
Removed goalkeepers duw to different foul profile/role.
Removed players with fewer than 1.0 '90s' played to avoid unstable per 90s rate from small sample
Computed Fouls per 90 using Fls/90s
Splitted players into two groups: Young(<=23) and Older (>23)

Data Preparation and Sampling
Population : Players who played at least 1.0 90s at world cup 2026
Sampling: Random sampling performed separately within each grouo
Sample size: 30 younger and 30 older giving a total sample of 60 players
Reproducibility: A fixed random state of 42 was used

Descriptive Statistics
For each group we calculated
Count
Mean
Median
Standard Deviation
Variance
Min and Max
Q1, Q3 and IQR
A boxplot was also created to compare the distribution of fouls per 90 minutes between the two age groups

Inferential Statistics — 95% Confidence Interval
A 95% confidence interval was calculated for the mean fouls per 90 minutes for each age group using the t-distribution.

Inferential Statistics — Two-Sample t-Test
Test used: Welch's two-sample t-test.
Significance level: 0.05

Null hypothesis (H0):
There is no significant difference in the mean fouls per 90 minutes between younger and older players.

Alternative hypothesis (H1):
There is a significant difference in the mean fouls per 90 minutes between younger and older players.

Decision rule:
If p < 0.05 → Reject H0.
If p ≥ 0.05 → Fail to reject H0.

In our case:
p = 0.82 which is greater than 0.05 so we fail to reject H0.