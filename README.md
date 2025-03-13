# Data Cleaning and Exploratory Data Analysis (EDA) with the Penguins Dataset

This project demonstrates data cleaning, outlier removal, and exploratory data analysis using the **Penguins dataset** available in Seaborn. The following steps are covered:

- **Data Cleaning**
  - Inspecting dataset structure
  - Handling missing values
  - Removing duplicates
  - Outlier detection and treatment using the IQR method
  - Standardizing categorical values

- **Exploratory Data Analysis (EDA)**
  - **Univariate Analysis:** Histograms and boxplots for numerical variables (e.g., `bill_length_mm`, `body_mass_g`)
  - **Bivariate Analysis:** Scatter plots, bar plots, and violin plots to examine relationships between variables
  - **Multivariate Analysis:** Pair plots and correlation heatmaps for in-depth variable interactions

- **Saving the Cleaned Data**
  - Exporting the cleaned dataset to a CSV file for further analysis

## Data Cleaning

1. **Loading the Data**
   - Load the dataset using `sns.load_dataset('penguins')`.

2. **Inspecting the Data**
   - Print the head, info, and summary statistics to understand the dataset's structure.
   - Check for missing values.

3. **Handling Missing Values**
   - Replace missing numerical values with the median.
   - Replace missing categorical values with the mode.

4. **Removing Duplicates**
   - Identify and remove duplicate records.

5. **Outlier Removal**
   - Define a function using the IQR method to remove outliers for selected numerical columns.
   - Apply the function on columns like `bill_length_mm` and `body_mass_g`.

6. **Standardizing Categorical Data**
   - Convert categorical values (e.g., `sex` to lowercase, `island` to uppercase) for consistency.

## Exploratory Data Analysis (EDA)

### Univariate Analysis

- **Summary Statistics:**
  ```python
  print(df.describe())
