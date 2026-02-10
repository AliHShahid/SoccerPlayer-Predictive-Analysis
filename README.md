### EuroSoccer-RatingNet

EuroSoccer-RatingNet is a predictive modeling project that utilizes a single-layer neural network to estimate the overall rating of professional football players. By analyzing key performance metrics from the European Soccer Database, the model identifies correlations between physical attributes and professional proficiency.

### Project Overview
The primary objective of this study is to quantify how specific player attributes—Potential, Acceleration, Sprint Speed, Agility, and Stamina—contribute to a player's official FIFA overall rating. The implementation utilizes a regression-based neural network architecture to process high-dimensional sports data.

### Technical Stack
* **Database Management:** SQLite3 for relational data extraction.
* **Data Engineering:** Pandas and Scikit-Learn (MinMaxScaler) for normalization and feature engineering.
* **Deep Learning Framework:** TensorFlow/Keras for model architecture and training.
* **Visualization:** Matplotlib and Seaborn for statistical analysis and error distribution plots.

### Model Architecture
The network is designed as a Sequential model with a linear approach to regression:
* **Input Layer:** Designed for 5 feature dimensions.
* **Hidden Layer:** 10 neurons with linear activation to maintain the continuous nature of player ratings.
* **Output Layer:** Single neuron for the continuous target variable (Overall Rating).
* **Optimization:** Adam optimizer utilizing Mean Squared Error (MSE) loss.



### Results
The model successfully minimizes the Mean Absolute Error (MAE) relative to the target range of ratings. Performance is evaluated through a scatter plot analysis comparing the ground-truth FIFA ratings against the network's generated predictions.

### Execution
To replicate the findings:
1. Ensure the SQLite database is placed in the designated input directory.
2. Install dependencies: `pip install tensorflow pandas scikit-learn matplotlib seaborn`.
3. Execute the Jupyter Notebook to initiate the preprocessing and training pipeline.
