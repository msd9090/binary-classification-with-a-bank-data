Markdown

# Bank Subscription Prediction Model

This project is an R-based machine learning project designed to classify bank customer data and predict the likelihood of a customer subscribing to a term deposit (the variable `y`). The project was developed as part of the [Kaggle Playground Series S5E8](https://www.kaggle.com/competitions/playground-series-s5e8).

## 🚀 Project Overview
The model analyzes tabular data containing 750,000 records and 18 features, including customer age, job type, marital status, and account balance. 

### Key Steps:
1. **Data Exploration:** Understanding column structures and detecting missing values.
2. **Feature Engineering:** Creating custom features like `blue_collar_job` to improve classification.
3. **Data Visualization:** Using `ggplot2` to visualize job distributions and subscription rates.
4. **Machine Learning:** - **Rpart:** Recursive partitioning for decision trees.
   - **Naive Bayes:** Probabilistic classification.
   - **Random Forest:** Ensemble learning for high-accuracy predictions.

## 🛠 Libraries Used
The following R packages are required to run this project:
* `tidyverse` (dplyr, ggplot2, readr)
* `rpart` & `rpart.plot`
* `naivebayes`
* `randomForest`

## 📊 Dataset Features
The dataset includes several customer attributes:
- **Demographics:** `age`, `job`, `marital`, `education`.
- **Financials:** `balance`, `housing` (loan), `loan` (personal).
- **Campaign Info:** `contact` method, `duration` of call, `campaign` frequency.
- **Target:** `y` (binary classification: 0 = No, 1 = Yes).

## 📝 How to Use
1. Clone this repository.
2. Ensure R and RStudio are installed.
3. Place the `train.csv` and `test.csv` files in the expected directory (usually `../input/`).
4. Run the `.ipynb` or `.R` script to generate the `submission.csv` file.
2. How to Run the Project
Since your project is in a .ipynb (Jupyter Notebook) format using the R kernel, follow these steps:

Option A: Running on Kaggle (Recommended)
Go to the Playground Series S5E8 competition.

Click "New Notebook".

Go to File -> Import Notebook and upload your my-project-r-13.ipynb file.

Ensure the data sources include the competition dataset.

Click "Run All".

Option B: Running Locally (RStudio)
Install R: Download it from CRAN.

Install RStudio: Download the Desktop version from Posit.

Open the Project:

If you want to use the notebook format, install the IRkernel in R.

Alternatively, copy the code from the notebook cells into a new R Script (.R file).

Install Dependencies: Run this command in your R console:

R

install.packages(c("tidyverse", "rpart", "rpart.plot", "naivebayes", "randomForest"))
Update File Paths: Make sure the read_csv path points to where you saved the train.csv file on your computer.

Run: Select the code and press Ctrl + Enter (or Cmd + Enter on Mac).

3. Creating the Submission
The script ends by generating a submission.csv file. You can upload this file directly to Kaggle to see your score on the leaderboard.
