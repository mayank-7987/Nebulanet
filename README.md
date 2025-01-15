# Exoplanet Classification for Humanity's Future
This project tackles the Exoplanet-Hunting Challenge at Jigyasa '24, a physics festival by IIT BHU, and was awarded **1st Place** at the **Nebulanet Hackathon**.
The goal is to develop a machine learning model that accurately predicts habitable exoplanets based on astronomical data, potentially guiding future interstellar exploration and the search for a second home for humanity.
## Model Used

* **BaggingClassifier with XGBoost:** This ensemble learning approach leverages the strengths of both algorithms to achieve high classification accuracy.

## Key Points

* **Dataset:** The provided dataset for the challenge can be found [here](https://www.kaggle.com/competitions/exoplanet-hunting/data).
* **Optimized Data Preprocessing:**
  * Irrelevant features were removed for improved model efficiency.
  * Dimensionality was reduced using PCA (9 components, retaining 97.1% variance) for faster training.
  * Features were standardized with StandardScaler for better model convergence.
* **Robust Evaluation & Hyperparameter Tuning:**
  * Stratified K-fold cross-validation ensured reliable performance estimation.
  * The Hyperopt library was used to optimize hyperparameters to maximize model accuracy.
* **Class Imbalance Handling:**
  * The 'scale_pos_weight' parameter addressed class imbalance in the target variable, focusing on cost-sensitive learning.


## Results

Achieved a remarkable mean accuracy of **0.9927** across all folds, demonstrating exceptional performance in exoplanet classification. The predictions of the model are stored [here](https://github.com/Dream-Falls/Nebulanet/blob/main/submission.csv).
