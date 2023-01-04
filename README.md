# Advertising-A-B-testing


# Project overview

The company is trying new ad design to increase ad success.
To do so they made new creative advertising design with SmartAd brand and conduct an A/B test in which one group of users have been shown an old ad and another - new one.

- **Experiment Approach**

Our goal is to analyse the results of A/B test and figure out wherever new disign of ad affects the behavior of users in terms of responding to BIO questionnaire.

- **Null Hypothesis Hₒ: p = pₒ** - There is no significant difference between the ad success rate of both groups


- **Alternative Hypothesis Hₐ: p ≠ pₒ** - There is significant difference between the ad success rate of both groups.
Given we don’t know if the new design will perform better/worse/equal as our current design, we will perform a two-tailed test


- **Confidence Level:** 95% (α=0.05)


- **p** and **pₒ** stand for the conversion rate of the new and old design.

## Contents

### Project structure
- [Input data](https://github.com/LtvnSergey/Advertising-A-B-Testing/tree/main/data)
- [Notebook](https://github.com/LtvnSergey/Advertising-A-B-Testing/blob/main/notebooks/Advertising-A-B-Testing.ipynb)


### Data description
- Input data - csv file with following columns:

| Field  |Description  |
|--------|--------------|
| auction_id  | The unique id of the online user who has been presented the BIO. In standard terminologies this is called an impression id. The user may see the BIO questionnaire but choose not to respond. In that case both the yes and no columns are zero. |
| experiment | Which group the user belongs to - control or exposed |
| control | Users who have been shown a dummy ad |
| exposed | Users who have been shown a creative, an online interactive ad, with the SmartAd brand |
| date | The date in YYYY-MM-DD format |
| hour | The hour of the day in HH format |
| device_make | The name of the type of device the user has e.g. Samsung |
| platform_os | The id of the OS the user has |
| browser | The name of the browser the user uses to see the BIO questionnaire |
| yes | 1 if the user chooses the “Yes” radio button for the BIO questionnaire |
| no | 1 if the user chooses the “No” radio button for the BIO questionnaire |

