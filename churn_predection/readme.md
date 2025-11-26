# Customer Churn Prediction & Analysis

## Project Description
This project utilizes the Telco Customer Churn dataset to predict whether a customer will stop using a service. A Logistic Regression model was built to classify customers into "Churn" or "No Churn" categories and, critically, to identify the key features driving customer attrition.

## Project Workflow

* **Exploratory Data Analysis (EDA):** Analyzed the distribution of target variables and relationships between features such as tenure, contract type, and monthly charges.
* **Data Preprocessing:**
    * Converted the `TotalCharges` column to numeric, handling missing values by filling them with 0 (representing new customers).
    * Applied One-Hot Encoding to categorical variables (e.g., "Yes"/"No", "Fiber Optic") to prepare data for the model.
* **Model Building:** Implemented a Logistic Regression model using Scikit-Learn. This algorithm was selected for its interpretability regarding feature weights.
* **Evaluation & Interpretation:** Evaluated model accuracy and visualized feature importance coefficients to derive business insights.

## Tech Stack
* **Language:** Python
* **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn

## Key Findings
Analysis of the model coefficients yielded the following insights:
1.  **High Churn Risk:** Customers with **Fiber Optic** internet and **Electronic Check** payment methods showed the strongest positive correlation with churn.
2.  **Retention Drivers:** **Two-Year Contracts** and higher **Tenure** (months as a customer) showed the strongest negative correlation with churn, indicating high retention.
3.  **Service Impact:** Subscriptions to add-on services like **Tech Support** and **Online Security** are associated with lower churn rates.

## How to Run
1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/YOUR-USERNAME/customer-churn-prediction.git](https://github.com/YOUR-USERNAME/customer-churn-prediction.git)
    ```
2.  **Install dependencies:**
    ```bash
    pip install pandas numpy matplotlib seaborn scikit-learn
    ```
3.  **Execute the notebook:**
    Open the Jupyter Notebook file to view the analysis pipeline and results.