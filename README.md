# Sentiment-Analysis-Using-Bert

**Sentiment Analysis for Productivity Apps**

**Introduction**

This project focuses on conducting sentiment analysis for productivity-related apps by analyzing user reviews from the Google Play Store. Understanding customer sentiment is crucial for businesses to improve product quality and enhance customer satisfaction. The project utilizes natural language processing (NLP) techniques and a pre-trained BERT-based model to classify reviews into positive, negative, or neutral sentiments.

**Dataset Creation and Preprocessing**

Dataset Selection: Reviews were collected using the Google-Play-Scrapper library from HuggingFace. The focus was on productivity apps such as habit trackers, calendar apps, and to-do lists.
App Selection: App-Annie website was utilized to select top-ranked third-party productivity apps from the Google Play Store.
Dataset Preprocessing: Scraped data was converted into a structured format (review.csv). Irrelevant columns were removed, and rows with empty data were dropped. Ratings were mapped to sentiments: 1 and 2 as negative, 3 as neutral, and 4 and 5 as positive. Class imbalance was checked, and fortunately, the data was well balanced.

**Model Training and Evaluation**
Model Selection: The pre-trained "Bert-base-cased" model was chosen for sentiment analysis due to its effectiveness in processing text data.
Fine-tuning: The BERT model was fine-tuned on the custom dataset to adapt it to the specific task of sentiment analysis.
Performance Evaluation: The trained model achieved an accuracy of approximately 87%. Evaluation metrics such as accuracy and a confusion matrix were calculated to assess the model's performance.

**Deployment**
Gradio App: The trained sentiment analysis model was deployed on Gradio, allowing users to input text prompts and receive sentiment predictions. This user-friendly interface enables easy access to the sentiment analysis pipeline.

Repository Structure
Source Code Files: Includes ipynb file for dataset preprocessing, model development, and evaluation.
README.md: Detailed documentation describing the project, dataset creation process, model training, evaluation, and deployment instructions.

**Screenshots**: Screenshots or demonstrations of the Gradio interface and results.
![Screenshot 2024-02-20 132532](https://github.com/Arpit-Avasarmol/Sentiment-Analysis-Using-Bert/assets/88440241/f5110b8c-f7ae-4e4e-8388-cfef976ff5af)


**Acknowledgments**
Special thanks to HuggingFace for providing the Google-Play-Scrapper library and pre-trained BERT model.
Acknowledgment to App-Annie for providing insights into app rankings and categories.
License
This project is licensed under the MIT License.


