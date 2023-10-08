# tiktok
### Predicting TikTok Video Classifications: 'Claims' vs. 'Opinions'
## Overview
The goal of this project was to construct a logistic regression and random forest model that can be used to determine if a TikTok video contains a claim or an opinion, to make the lives of employees easier when sorting through reported videos. The final random forest model had 100% accuracy and 100% precision in predicting the features that are most important in determining if a video will be classified as a claim or an opinion. According to the model, the factors that had the most influence in determining video classification were factors related to user engagement including video downloads, views, likes, and shares.
## Business Understanding
TikTok is a very popular short-form video app that allows users to post their own original content and engage with others (tiktok.com). Videos posted to TikTok must adhere to their Community Guidelines, and if a video does not adhere to this users are able to report them for violations, where they will be reviewed and either okayed or removed from the app. Read more about TikTok's content violations and bans [here](https://support.tiktok.com/en/safety-hc/account-and-user-safety/content-violations-and-bans#).
## Data Understanding
The data from this project is comprised of synthetic data created for the Google Advanced Data Analytics Certificate in partnership with TikTok. The dataset contains 19,383 unique observations and 12 features. Features in the dataset include information on user engagement, information about the video, author ban stauts, and claim status. In this model, there was no need to perform feature engineering, and columns were dropped or reformatted to fit the model.
## Modeling and Evaluation
The random forest model was used to determine feature importance in classifying TikTok videos as claims or opinions. The following plot shows that the most important features in separating a claim video from an opinion video are video view count, like count, share count, and download count. The final model had 100% accuracy and 100% precision, making it extremely effective at separating claims from opnions. Feature engineering was not necessary because the model is performing exceptionally well already.

<img width="567" alt="Screenshot 2023-10-07 at 7 44 39 PM" src="https://github.com/allisonlmueller/tiktok/assets/147258601/aa336b5e-81a6-4458-ada2-ecbecca38d46">

## Conclusion
This model would be very effective at helping the staff at TikTok determine if videos are claims or opinions, reducing the amount of videos that humans have to sort through and classify. Although new features did not need to be engineered due to the model's high performance, it might be helpful to have the number of reports for all videos posted by each author.
