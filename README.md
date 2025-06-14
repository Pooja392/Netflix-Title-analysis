# 📊 Netflix Titles Dataset Analysis and Prediction

This project performs **Exploratory Data Analysis (EDA)** and **basic prediction modeling** on the Netflix Titles dataset. The goal is to gain insights from the data and build a simple prediction model to classify content types.

---

## 📁 Dataset Information

The dataset contains information about movies and TV shows available on Netflix. Key columns include:

- `show_id`: Unique identifier
- `type`: Movie or TV Show
- `title`: Name of the content
- `director`: Director’s name
- `cast`: Main cast
- `country`: Country of origin
- `date_added`: Date it was added to Netflix
- `release_year`: Year of release
- `rating`: Content rating (e.g., TV-MA, PG)
- `duration`: Length of movie/show
- `listed_in`: Genre(s)
- `description`: Short summary

---

## 🧪 Technologies Used

- **Python 3**
- **Pandas** – data manipulation and analysis
- **NumPy** – numerical operations
- **Matplotlib & Seaborn** – data visualization
- **Scikit-learn** – machine learning model

---

## 🧼 Data Cleaning Steps

- Handled missing values using `fillna()` and `dropna()`
- Removed duplicate rows
- Used `isnull().sum()` to detect missing data
- Filled missing values for:
  - `country`, `cast`, `director` → 'Unknown'
  - `rating` → Mode (most frequent rating)
- Extracted numeric values from `duration`
- Created a new column `duration_type` from the text (e.g., "min", "Seasons")

---

## 📊 Exploratory Data Analysis (EDA)

We performed various analyses such as:

- Count of Movies vs TV Shows
- Year-wise content release and addition
- Most common ratings (e.g., TV-MA, PG)
- Top countries producing Netflix content
- Frequent genres and categories
- Average duration by type and rating
- Grouped aggregations

### 📈 Visualizations

- Bar plots for content types and ratings
- Pie charts for duration types
- Line plots for year-wise trends
- Aggregated plots using `groupby` and `agg()`

---

## 📉 Aggregation Operations

We performed various statistical aggregations:

- **count()** – Number of entries
- **sum()** – Total (where applicable)
- **mean()** – Average values
- **median()** – Middle value
- **min(), max()** – Minimum and maximum values
- Grouped aggregations using `groupby()` with multiple columns

## Author - Pooja Patil
