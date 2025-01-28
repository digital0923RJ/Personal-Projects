## 1. Crop Image Classification

- Initially, the project focused on classifying five types of crops. While I wanted to include more, limited GPU resources constrained further expansion. Feature engineering was completed using techniques such as data augmentation, image normalization, and one-hot encoding.

- Model training was optimized using Optuna to identify the best hyperparameters, and training was conducted using VGG19 via transfer learning. The VGG19 model was analyzed layer by layer, and specific top layers were extracted, recompiled, and fine-tuned to enhance model performance.

- To monitor overfitting, accuracy and loss were visualized throughout the training process. Additionally, a confusion matrix was generated to evaluate and visualize the model's performance on the training data.

- This approach ensured a robust and efficient image classification pipeline.

## 2. Coin AI Automated Trading Algorithm (Dogecoin)

-  The trading algorithm uses a volatility breakout strategy optimized with a parameter k, which is determined by maximizing cumulative returns. Real-time trading is supported with PyUpbit API for Dogecoin. Key features include:
   -  10-day Moving Average (MA10): Used to confirm trends.
   -  Real-time Price Monitoring: Fetches the current price to decide buy/sell actions.
   -  Automated Buy/Sell Logic: Trades based on target price and MA10.
   -  Account Balance Management: Ensures safe trading thresholds.

-  The algorithm processes real-time data, requiring scalable and reliable infrastructure. For this, AWS EC2 is utilized to run the trading bot continuously in a cloud environment, ensuring consistent performance and availability.
