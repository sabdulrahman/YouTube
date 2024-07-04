YouTube and Science: Models for Research Impact

Summary: The research explores the growing intersection of YouTube videos and academic research citations, highlighting increased video references to scholarly articles. To analyze this trend, new datasets were created, and machine-learning models were developed to predict citation patterns and the influence of video views on the popularity and public engagement of research articles.

Abstract: Video communication has rapidly increased over the past decade, with YouTube providing a medium where users can post, discover, share, and react to videos. There has also been an increase in the number of videos citing research articles, especially since it has become relatively commonplace for academic conferences to require video submissions. However, the relationship between research articles and YouTube videos is unclear, and the present paper aims to address this issue. We created new datasets using YouTube videos and mentions of research articles on various online platforms. Most of the articles cited in the videos are related to medicine and biochemistry. We analyzed these datasets through statistical techniques and visualization and built machine learning models to predict (1) whether a research article is cited in videos, (2) whether a research article cited in a video achieves a level of popularity, and (3) whether a video citing a research article becomes popular. The best models achieved F1 scores between 80% and 94%. According to our results, research articles mentioned in more tweets and news coverage are more likely to receive video citations. We also found that video views are essential for predicting citations and increasing research articles’ popularity and public engagement with science.

![Data process](https://github.com/sabdulrahman/YouTube/blob/main/data.png)

Dataset:

The dataset aims to facilitate further investigation into the impact of YouTube videos on both the scientific community and the general public.

  DatasetA1 - Contains Altmetric IDs and metadata for articles cited in YouTube videos.
  DatasetB - Comprises YouTube links to videos that have cited articles.
  DatasetC1 - A merged dataset focusing on the research articles cited in the videos.
  DatasetC2 - A merged dataset concentrating on the YouTube videos that cited the articles.

Coding Files: 

Coding Files Descriptions:

1. extract_altmetric_data.py - Script to extract altmetric data via the Altmetric API and Beautiful Soup.
2. extract_youtube_data_using_selenium.py - Script to extract metadata such as likes, dislikes, subscriber name, subscriber count, and views from a YouTube video using Selenium.
3. get_youtube_links_using_cookies.py - Script to extract YouTube links from altmetric records using Altmetric IDs, requiring cookies or login credentials for Altmetric.
4. identify_unavailable_videos.py - Code to check for unavailable YouTube videos using links through Selenium.
5. making_combined_csv.py - Code to merge two CSV files using a standard ID as the key.
6. predicting_subjects_multilabel_classification - Details model results for predicting the subjects of research articles cited in a video, utilizing altmetric and YouTube data. Models implemented include Logistic Regression with BinaryRelevance, Random Forest with LabelPowerset, and Logistic Regression with a One-vs-Rest approach. It also uses LDA for subject prediction from abstract topics, achieving an F1 score of 0.82.
7. predicting_the_youtube_category - Showcases model outcomes trained to categorize YouTube videos into 7 categories using altmetric and YouTube data. Includes models like Random Forest (F1-score of 0.67), Logistic Regression, and Decision Tree.
8. Views_per_day_model - Displays results from a model that predicts daily views of a YouTube video based on altmetric features.

Paper: https://link.springer.com/article/10.1007/s11192-022-04574-5

Shaikh, Abdul Rahman, Hamed Alhoori, and Maoyuan Sun. "YouTube and science: models for research impact." Scientometrics 128, no. 2 (2023): 933-955.
