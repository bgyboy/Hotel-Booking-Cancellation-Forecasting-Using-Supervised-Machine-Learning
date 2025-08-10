Hotel Booking Cancellation Prediction
=====================================

Project Overview
----------------
This project analyzes hotel booking data to identify patterns in guest behavior, understand factors affecting cancellations, and build predictive models to classify whether a booking will be canceled or honored.

Dataset
-------
The dataset contains hotel booking details, including:
- Booking information (hotel type, arrival date, lead time, market segment)
- Guest details (number of adults, children, babies, country)
- Stay details (weekend/weeknight stays, room types, special requests)
- Financial details (average daily rate)
- Booking outcomes (is_canceled, reservation status)

Main Tasks Performed
--------------------
1. Data Cleaning
   - Handled missing values using interpolation and imputation.
   - Corrected logically inconsistent records (e.g., bookings with zero guests).

2. Exploratory Data Analysis (EDA)
   - Spatial analysis of guest origins by country.
   - Analyzed per night price per person (box plots).
   - Studied room price variation over the year.
   - Identified busiest months for both resort and city hotels.
   - Analyzed average length of stay.
   - Correlation analysis to find important numerical features for predicting cancellations.
   - Outlier detection and handling to improve model accuracy.

3. Feature Engineering
   - Encoded categorical variables using One-Hot Encoding.
   - Selected important features based on correlation and domain logic.
   - Scaled numerical variables for algorithms sensitive to distances.

4. Machine Learning Model Building
   - Target variable: is_canceled (1 = canceled, 0 = not canceled).
   - Models implemented:
     * Naive Bayes
     * K-Nearest Neighbors (KNN)
     * Decision Tree Classifier
     * Random Forest Classifier
   - Evaluation metrics:
     * Accuracy
     * Precision
     * Recall
     * F1-score
     * Confusion Matrix

Key Insights
------------
- Lead time, ADR (Average Daily Rate), and previous cancellations are strong predictors of booking cancellation.
- Prices vary seasonally, with noticeable peaks during holiday seasons and summer.
- Resort and city hotels have different patterns for peak booking months.

Project Structure
-----------------
- Data Cleaning and Preprocessing
- Exploratory Data Analysis (EDA)
- Feature Engineering
- Model Training and Evaluation
- Results and Insights

Requirements
------------
- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn

How to Run
----------
1. Clone the repository.
2. Install required dependencies using:
   pip install -r requirements.txt
3. Run the Jupyter Notebook or Python script to reproduce results.

Author
------
Ayush Kumar

