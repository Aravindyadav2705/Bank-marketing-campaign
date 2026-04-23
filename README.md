# Machine Learning in Customer Subscription of Bank Term Deposits

## 1. Abstract
This project evaluates the efficiency of machine learning in predicting customer subscriptions for bank term deposits using the UCI Bank Marketing dataset . The study implemented four specific models: **Logistic Regression**, **Multi-Layer Perceptron (MLP)**, **Deep Artificial Neural Network (Deep ANN)**, and **Residual Network (ResNet)** . Performance was evaluated using accuracy, precision, recall, and F1-score . Results show that advanced architectures (Deep ANN and ResNet) achieve superior accuracy and precision (~90%), while the baseline Logistic Regression model yields higher recall (~78%) and better interpretability . Campaign-related features, notably call duration and prior outcomes, were identified as the most predictive factors .

## 2. Methodology
The project follows a structured machine learning pipeline:
* **Baseline**: Logistic Regression was established for its high interpretability and suitability for binary classification .
* **Neural Network (MLP)**: A feed-forward architecture with layers of 64 and 32 neurons was implemented to capture non-linear relationships .
* **Deep ANN**: A Keras-based model utilizing Batch Normalization and Dropout layers was built to optimize performance and mitigate overfitting .
* **ResNet**: A Residual Network architecture was employed, using skip connections to enhance gradient flow and learn subtle patterns in tabular data .

## 3. Results and Performance Analysis
The predictive capabilities of the models were quantified as follows :
* **Logistic Regression**: Achieved an accuracy of 90% and a recall of 32.23%, prioritizing lead identification over precision .
* **Deep ANN**: Passed the performance threshold with a peak accuracy of 90.58%, successfully filtering out non-subscribers with high precision .
* **ResNet**: Maintained a steady accuracy of approximately 90.28%, balancing precision and recall through residual learning .
* **MLP**: Reached an accuracy of 90.34%, providing a balanced classification across demographics .

## 4. Analysis and Discussion
The findings reveal distinct trade-offs between accuracy and interpretability . While Deep ANN and ResNet offer higher predictive power, Logistic Regression remains the most transparent, allowing for direct coefficient analysis—a critical requirement in regulated banking sectors . In all models, behavioral metrics such as **call duration** and **previous campaign results** proved to be the strongest predictors of subscription success . The inherent class imbalance (~88% non-subscribers) remains a limitation, influencing model bias despite class-weighting adjustments .

## 5. Conclusion
This study demonstrates that machine learning can effectively optimize bank marketing campaigns. For lead volume, Logistic Regression is optimal due to high recall; for operational efficiency and cost-saving, Deep ANN or ResNet architectures are superior due to higher precision and lower false-positive rates .
