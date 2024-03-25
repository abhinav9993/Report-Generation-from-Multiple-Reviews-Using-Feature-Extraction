# Report-Generation-from-Multiple-Reviews-Using-Feature-Extraction

As the digital landscape evolves, the surge in customer reviews necessitates automating the review analysis process to provide valuable insights for both consumers and manufacturers. This project focuses on enhancing feature extraction and sentiment analysis to create informative summaries from customer feedback.

## Approach
The project's architecture involves three main steps:

### 1. Review Cleaning
- Emojis are disregarded, and the dataset is demojified for further processing.
- Reviews with a minimum word length of two are considered meaningful.
- Single-word reviews are eliminated, while two-word reviews lacking a (noun+adjective) pair are removed.
- All reviews are converted to lowercase to ensure consistency during POS tagging.

### 2. Frequent Feature Identification
- The project mines frequent features explicitly mentioned in reviews.
- Techniques like POS tagging, Association Rules mining, and Feature Pruning are employed for feature identification.
- Spelling correction using Levenshtein's distance is integrated to handle minor errors.

### 3. Opinion Mining and Sentiment Scoring
- Explicit opinions are focused on, assuming a single opinion per feature in a sentence.
- The nearest opinionated phrase to a feature is extracted for sentiment analysis.
- Sentiment scores are calculated using VADER for polarity extraction, determining the sentiment towards each feature.

## Conclusion
This project proposes a pipeline for extracting meaningful features from customer reviews and assigning sentiment scores to each feature. The pipeline comprises cleaning, feature extraction, and opinion mining stages. By evaluating the method on smartphone reviews, meaningful results were obtained, aiding in understanding customer sentiments towards specific product features.

This approach enhances the understanding of customer feedback by extracting key features and sentiments from reviews, providing valuable insights for decision-making processes in e-commerce and product development.
