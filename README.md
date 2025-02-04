# YouTube and Science: Models for Research Impact

## Overview
This project analyzes the relationship between YouTube videos and research articles to understand their societal and scholarly impact. The project involves data extraction, analysis, and predictive modeling using machine learning techniques.

### Data Collection and Processing Scripts
- **extract_altmetric_data.py**: Extracts research article metadata and altmetric mentions from online platforms.
- **extract_youtube_data_using_selenium.py**: Scrapes YouTube data using Selenium.
- **get_all_unique_youtube_ids.py**: Identifies and stores unique YouTube video IDs.
- **get_youtube_links_using_cookies.py**: Retrieves YouTube video links that cite research articles.
- **identify_unavailable_videos.py**: Detects and removes unavailable videos from the dataset.
- **making_combined_csv.py**: Combines multiple datasets into a single CSV file for analysis.

### Machine Learning and Analysis Notebooks
- **predicting_subjects_multilabel_classification.ipynb**: Implements a multi-label classification model to predict research subjects.
- **predicting_the_youtube_category.ipynb**: Uses machine learning to categorize YouTube videos based on their content.
- **views_per_day_model.ipynb**: Develops a predictive model to estimate the number of daily views for YouTube videos citing research articles.

## Methodology
1. **Data Collection**: Extracting research articles and their citations in YouTube videos using Altmetric and YouTube APIs.
2. **Preprocessing**: Cleaning and structuring data, handling missing values, and normalizing features.
3. **Exploratory Data Analysis**: Visualizing trends in YouTube citations of research papers.
4. **Machine Learning Models**:
   - Predicting whether a research article will be cited in a YouTube video.
   - Estimating the impact of video citations on scholarly citations.
   - Predicting video popularity based on research article metadata.

## Results
- Research articles in the fields of Medicine and Biochemistry are cited the most in YouTube videos.
- Videos categorized as Science & Technology and Education have the highest view counts.
- Altmetric mentions, including Twitter and news coverage, significantly impact video citations.
- Machine learning models achieved high accuracy in predicting video citations, scholarly impact, and video views.

## Future Work
- Incorporating textual and temporal features from both research articles and video descriptions.
- Analyzing the reasons for citing research in videos, such as educational purposes, news dissemination, or commercial use.
- Extending the analysis to include other social media platforms for broader altmetric insights.

## References
For a detailed discussion of the methodology and findings, refer to the research paper: [YouTube and Science: Models for Research Impact](https://link.springer.com/article/10.1007/s11192-022-04574-5).

## Collaboration
For inquiries, collaboration opportunities, please reach out to me or connect via professional networks. [Website](sabdulrahman.github.io)
