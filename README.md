------NLP ASSIGNMENT--------


OUTPUT IS IN THE LAST









Sentiment Analysis with Custom PyTorch Model + Hugging Face Integration
=======================================================================

Overview
--------
This project combines a Hugging Face sentiment analysis pipeline with a custom PyTorch neural network for multi-class sentiment prediction. It uses:
- **Hugging Face (Transformers)** to fetch sentiment scores from text comments.
- **PyTorch** to create a neural network model that predicts sentiment based on QoS (Quality of Service) data and sentiment scores.
- **scikit-learn (StandardScaler)** to standardize input features.

The model classifies inputs into three categories:
1. Negative
2. Neutral
3. Positive

Components
----------
- **SentimentModel (PyTorch class)**: A simple feedforward neural network with one hidden layer.
- **get_sentiment_score(comment)**: Uses Hugging Face’s `distilbert-base-uncased-finetuned-sst-2-english` model to analyze comment sentiment.
- **predict_sentiment_with_model(comment)**: Integrates the Hugging Face sentiment score with simulated QoS data and makes a prediction using the custom model.
- **Training block**: Simulates training data, trains the PyTorch model, and scales the data using `StandardScaler`.
