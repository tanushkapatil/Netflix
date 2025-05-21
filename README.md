# Netflix Movie Popularity Classification

This project analyzes a Netflix movies dataset to explore movie genres, popularity, and other factors, and builds a machine learning model to classify movie popularity levels.

---

## Project Overview

- **Objective:**  
  Perform Exploratory Data Analysis (EDA) on Netflix movies data, visualize key insights, and build a Random Forest classifier to predict the popularity category of movies.

- **Dataset:**  
  Contains Netflix movies metadata including genre, release date, popularity score, vote average, and vote count.

---

## Key Steps

### Data Preprocessing
- Loaded and explored the dataset.
- Converted release date to year format.
- Dropped irrelevant columns (`Overview`, `Original_Language`, `Poster_Url`).
- Handled duplicates and missing values.
- Split multi-genre entries into individual rows.
- Categorized `Vote_Average` into quartile-based labels.
- Created a target label based on popularity thresholds:  
  - `popular`  
  - `average`  
  - `unpopular`

### Exploratory Data Analysis (EDA)
- Visualized genre distribution and frequency.
- Analyzed genres with highest average votes.
- Identified movies with highest and lowest popularity.
- Examined year-wise movie release trends.

### Machine Learning
- Selected features: `Vote_Average`, `Vote_Count`, `Popularity`.
- Encoded categorical variables and target labels.
- Balanced the dataset using downsampling techniques.
- Split data into training and testing sets.
- Trained a Random Forest Classifier.
- Evaluated model performance with accuracy, classification report, and confusion matrix.

---

## Results

- **Model Accuracy:** 100% on test set.
- **Classification Report:**  
  Perfect precision, recall, and F1-score across all popularity classes.
- **Confusion Matrix:**  
  No misclassifications; model predicted all samples correctly.

---

## Dependencies

- Python 3.12.17
- pandas
- numpy
- seaborn
- matplotlib
- scikit-learn

---

## How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/tanushkapatil/Netflix-Data-Analysis.git
