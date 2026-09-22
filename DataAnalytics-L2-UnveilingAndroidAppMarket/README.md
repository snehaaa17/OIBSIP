# Unveiling the Android App Market
## Google Play Store Analysis

**OASIS INFOBYTE – Data Analytics Internship**  
## Level 2-Task 4
  
**Project:** Unveiling the Android App Market (Google Play Store Analysis)

---

## Project Overview

This project analyzes Google Play Store application data to understand different patterns in the Android app market.

The analysis focuses on application categories, ratings, reviews, installs, app size, pricing, estimated revenue, and user sentiment. Python and data visualization techniques were used to clean the datasets, explore the data, identify patterns, and present the findings through charts and interactive visualizations.

Two datasets were used in this project:

- `googleplaystore.csv` – information about Google Play Store applications
- `googleplaystore_user_reviews.csv` – user reviews and sentiment-related information

---

## Objectives

The main objectives of this project are:

- Clean and prepare the Google Play Store datasets.
- Analyze the distribution of applications across categories.
- Study the distribution of application ratings.
- Compare average ratings between categories.
- Examine the relationship between app size and installs.
- Analyze free and paid applications.
- Study the price distribution of paid applications.
- Estimate revenue using application price and install information.
- Perform sentiment analysis on user reviews.
- Compare sentiment across application categories.
- Create an interactive visualization using Plotly.
- Derive useful insights from the analysis.

---

## Datasets

### Google Play Store Apps Dataset

The application dataset contains information such as:

- App name
- Category
- Rating
- Number of reviews
- Number of installs
- App size
- Type
- Price
- Content rating
- Genres
- Last updated date
- Current version
- Android version

### Google Play Store User Reviews Dataset

The review dataset contains information such as:

- App name
- Translated review
- Sentiment
- Sentiment polarity
- Sentiment subjectivity

---

## Data Cleaning and Preparation

Before performing the analysis, the datasets were inspected and cleaned.

The major preprocessing steps included:

- Checking missing values.
- Removing duplicate records.
- Converting the `Reviews` column into a numeric format.
- Cleaning the `Installs` column by removing commas and the `+` symbol.
- Converting application size into MB where possible.
- Handling missing values required for specific analyses.
- Checking duplicate application names.
- Removing unsuitable review records before sentiment analysis.
- Combining application and review data for category-wise sentiment analysis.

After cleaning, the application dataset contained **9,659 records** and the review dataset used for sentiment analysis contained **29,692 records**.

---

## Analysis Performed

### 1. Category Analysis

The number of applications in each category was calculated and visualized using a bar chart.

The cleaned dataset contains **33 application categories**.

The categories with the highest number of applications were:

- **Family:** 1,832
- **Game:** 959
- **Tools:** 827

The distribution shows that applications are not equally distributed across all categories.

---

### 2. Ratings Analysis

The distribution of application ratings was analyzed using a histogram.

The average rating in the cleaned rating data was approximately:

**4.17**

Average ratings were also calculated for individual categories and represented using a category-wise bar chart.

---

### 3. App Size vs Installs

A scatter plot was created to examine whether application size is related to the number of installs.

The calculated correlation coefficient was:

**0.1343**

This represents a weak positive relationship between app size and installs in the analyzed dataset. Therefore, app size by itself does not provide a strong explanation for differences in installation counts.

---

### 4. Pricing Analysis

Applications were divided into free and paid applications.

The cleaned dataset contained:

| Type | Number of Apps | Percentage |
|------|----------------|------------|
| Free | 8,902 | 92.17% |
| Paid | 756 | 7.83% |

The price distribution of paid applications was also analyzed using a histogram.

Most paid applications were concentrated toward the lower end of the price range, while a smaller number of applications had considerably higher prices.

---

### 5. Estimated Revenue Analysis

A simple estimated revenue measure was calculated using:

`Estimated Revenue = Price × Installs`

The result was aggregated by category to compare the estimated values between different categories.

This is only an analytical estimate based on the available price and install information. It should not be considered actual revenue because factors such as platform fees, refunds, discounts, taxes, and other business costs are not included.

---

### 6. User Review Sentiment Analysis

VADER sentiment analysis was used to classify user reviews into positive, negative, and neutral categories.

The sentiment results were:

| Sentiment | Reviews | Percentage |
|-----------|---------|------------|
| Positive | 20,195 | 68.01% |
| Negative | 5,867 | 19.76% |
| Neutral | 3,630 | 12.23% |

Positive reviews represented the largest share of the analyzed reviews.

---

### 7. Sentiment by Category

The application and review datasets were combined to study sentiment across different application categories.

The analysis showed that sentiment percentages vary between categories.

For example, the categories with relatively high positive sentiment included:

- Comics
- Auto and Vehicles
- Events
- Education
- Health and Fitness

Categories with comparatively higher negative sentiment included:

- Video Players
- Social
- Entertainment
- News and Magazines
- Communication

These differences provide useful information about how user feedback varies between different types of applications.

---

### 8. Interactive Visualization

Plotly was used to create an interactive visualization of average application ratings by category.

The interactive chart allows the viewer to explore category-wise ratings and view additional information through the chart interface.

---

## Key Findings

The major findings from this analysis are:

1. The Family, Game, and Tools categories contain the largest number of applications in the cleaned dataset.

2. The overall average application rating is approximately **4.17**, indicating that the ratings in the dataset are generally concentrated toward the higher end of the rating scale.

3. Free applications make up approximately **92.17%** of the cleaned application dataset, while paid applications account for approximately **7.83%**.

4. The correlation between app size and installs is approximately **0.1343**, showing only a weak positive relationship.

5. Sentiment analysis classified approximately **68.01%** of the analyzed reviews as positive, **19.76%** as negative, and **12.23%** as neutral.

6. User sentiment differs across application categories, showing that feedback patterns are not the same for every category.

---

## Tools and Technologies

The following tools and libraries were used:

- **Python**
- **Jupyter Notebook**
- **Pandas**
- **NumPy**
- **Matplotlib**
- **Seaborn**
- **Plotly**
- **VADER Sentiment**

---

## Project Files

```text
DataAnalytics-L2-UnveilingAndroidAppMarket/
│
├── README.md
├── Google_Play_Store_Analysis_Task3.ipynb
├── googleplaystore.csv
└── googleplaystore_user_reviews.csv
