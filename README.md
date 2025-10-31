# Data preprocessing made simple 

# Importing Libraries
---> Used pandas for data handling and manipulation.
---> Used Scikit-learn for Feature Scaling

# Time Series Data
---> Loaded the Financials dataset using parse_dates for the Date column and set it as the index to prepare for time series analysis.

# Finding Missing Values
---> Checked missing values using df.isna().sum() to understand data completeness.
---> In this preprocessing process I handled missing values using

   - interpolate()
   - mean ()
   - median ()
   - randint ()
   - ffill ()
   - bfill ()        

# Finding Duplicates
---> Used df.duplicated().sum() to detect any duplicate rows in the dataset.

# Dropping Unnecessary Columns
---> Removed columns like Month Number, Month Name, and Year since the Date index already contains that information.

# Data Overview
---> Used df.info() and df.describe() to understand data types, memory usage, and summary statistics.

# Exploring Unique Values
---> Checked unique entries in columns like Segment, Country, Product, and Discount Band to understand categorical distributions.

# Type Casting (Data Cleaning)
---> Cleaned all numeric columns (like Units Sold, Manufacturing Price, Sale Price, Gross Sales, Discounts, Sales, COGS, and Profit) by removing unwanted symbols like $, ,, or % and converted them to float.

# Handling Missing or Invalid Values
---> Used .fillna(0) and errors='coerce' to safely handle non-numeric or missing values.

# Final Output
---> Saved the cleaned dataset to Processed_Financials.csv for further use.
