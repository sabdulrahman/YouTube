YouTube and Science: Models for Research Impact

Summary: The research explores the growing intersection of YouTube videos and academic research citations, highlighting increased video references to scholarly articles. To analyze this trend, new datasets were created, and machine-learning models were developed to predict citation patterns and the influence of video views on the popularity and public engagement of research articles.

Abstract: Video communication has rapidly increased over the past decade, with YouTube providing a medium where users can post, discover, share, and react to videos. There has also been an increase in the number of videos citing research articles, especially since it has become relatively commonplace for academic conferences to require video submissions. However, the relationship between research articles and YouTube videos is unclear, and the present paper aims to address this issue. We created new datasets using YouTube videos and mentions of research articles on various online platforms. We found that most of the articles cited in the videos are related to medicine and biochemistry. We analyzed these datasets through statistical techniques and visualization and built machine learning models to predict (1) whether a research article is cited in videos, (2) whether a research article cited in a video achieves a level of popularity, and (3) whether a video citing a research article becomes popular. The best models achieved F1 scores between 80% and 94%. According to our results, research articles mentioned in more tweets and news coverage are more likely to receive video citations. We also found that video views are essential for predicting citations and increasing research articles’ popularity and public engagement with science.

Coding Files: 

1. extract_altmetric_data.py - Script to extract altmetric data using Altmetric API and Beautiful Soup.
2. extract_youtube_data_using_selenium.py - Script to extract metadata (likes, dislikes, subname, subno, views, etc..) from a Youtube video using selenium through link.
3. Views_per_day_model - Results of the model trained to predict views per day of the YouTube video using altmetric features.
4. predicting_the_youtube_category - Results of the model trained to predict the category (7 categories) of a YouTube video using altmetric and YouTube features. Built models for Random Forest (0.67 F1- score), Logistic Regression, and Decision Tree.
5. predicting_subjects_multilabel_classification - Results of the model trained to predict the subjects of a research article cited in video using altmetric and YouTube features. Built models Logistic Regression with BinaryRelevance, Random Forest with LabelPowerset, and Logistic Regression with one Vs rest approach. We then used topics from the abstract using LDA to predict the subjects achieving an F1-score of 0.82.
6. making_combined_csv.py - Code to combine two csv files based on a standard ID.
7. identify_unavailable_videos.py - Code to identify unavailable videos on YouTube through links using selenium.
8. get_youtube_links_using_cookies.py - Script to extract youtube links from altmetric using altmetric IDs (need cookie or login credential for altmetric)

Paper: https://link.springer.com/article/10.1007/s11192-022-04574-5
