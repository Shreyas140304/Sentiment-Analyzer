# Sentiment-Analyzer
Engineered a data pipeline using the Google YouTube Data API and a Random Forest classifier to preprocess and categorize thousands of user comments into positive, negative, and neutral sentiments, with pattern-extraction via regular expressions to surface feature requests and actionable insights (accuracy up to 80%)

YouTube Comment Sentiment & Pattern Analysis

Overview This project implements a scalable pipeline to collect, preprocess, and analyze user feedback from YouTube. It combines automated data acquisition with classical machine learning and pattern-extraction techniques to produce sentiment labels and surface actionable comment categories.

Key components

- **Data acquisition:** Automated collection of thousands of comments using the Google YouTube Data API, with pagination, rate-limit handling, and metadata capture (author, timestamp, video id).
- **Preprocessing:** Text cleaning (lowercasing, punctuation removal, basic stopword handling), token normalization, and removing duplicates to prepare data for modeling.
- **Feature Engineering:** Used TF-IDF vectorizer to convert the sentence to a vector form and get the rare or the dominant word in the text a high score.
- **Classification engine:** Random Forest classifier trained to categorize comments as positive, negative, or neutral, achieving up to 80% accuracy on held-out validation data.
- **Pattern extraction:** Regular-expression rules to detect explicit mention types such as postive like your videos are very inspiring and intersting, Negative like bug reports or not happy with the content and finally the neutral ones, where the comments not good nor bad in sound. 
- **Analytics & insights:** Aggregated dashboards and reports that provide categorical overviews by video/aspect and highlight which aspects deserve attention based on sentiment and frequency.

**Results**
1. Processed and labeled thousands of comments.
2. Achieved classification accuracy up to 80%.
3. Extracted targeted patterns (e.g., feature requests) to guide product and content decisions.
4. Technologies Google YouTube Data API, Python, scikit-learn (Random Forest), pandas, regex, (optionally) Jupyter, and plotting libraries for visualization.

**Possible next steps..**

- Improve classification with transformer-based models or ensemble approaches.
- Expand pattern extraction with named-entity recognition or dependency parsing to capture nuanced requests.
- Add a small user interface/dashboard for stakeholders to explore insights by video/timeframe.
