# dsci-100-project_template
### Predicting Newsletter Subscription from Player Characteristics

Summary: 
This project explored whether a player's age, total hours played, and self-reported experience level could be used to predict newsletter subscription behavior on a Minecraft server operated by UBC’s Pacific Laboratory for Artificial Intelligence (PLAI). Using a dataset of players, the analysis focused on classifying subscription status (TRUE/FALSE) through a K-Nearest Neighbors (KNN) classification model. Data were preprocessed by removing irrelevant fields, handling missing values, and splitting into training and testing sets (75/25). Exploratory analysis showed that subscribers tended to be younger and played more hours, while experience level had little predictive value. Initial modeling without correcting class imbalance led to high accuracy (up to ~81%) but failed to identify non-subscribers, defaulting to majority-class prediction. After applying upsampling to balance the classes, accuracy dropped to ~57.1%, but the model became better at detecting both subscribed and non-subscribed players. Despite the modest accuracy, the project revealed that current features alone were not sufficient for strong predictive performance. The author suggests adding richer behavioral metrics and testing alternative models (e.g., logistic regression or random forest) for future improvements.

Key Findings: 
- Subscribers were on average younger and played more.
- The initial model overfit to the majority class (subscribers).
- Upsampling improved class balance but reduced overall accuracy.
- Experience level was not a meaningful predictor.
- Final model accuracy: ~57.1%

Future Directions: 

- Add features like login frequency, session times, or in-game interactions.
- Test other classification algorithms.
- Evaluate precision-recall trade-offs depending on marketing goals.