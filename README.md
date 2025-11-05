# EdTech Analysis Dashboard - Power BI Project

This repository contains a Power BI portfolio project analyzing an EdTech (Online Courses) dataset. The goal is to provide actionable insights for a business to improve its content strategy, learner engagement, and course offerings.

## Dashboard Snapshot

Here is a high-level view of the final interactive dashboard.

<img width="755" height="764" alt="image" src="https://github.com/user-attachments/assets/8cd676b1-f372-465e-8de0-15a62acab9d3" />


## 📋 Problem Statement

The core task was to analyze a dataset of online courses to understand the key factors driving their success. The dashboard needed to answer critical business questions for a content manager, such as:
* What are the most popular course categories and types?
* What skills are currently in high demand?
* How do course duration, language, and subtitle count affect viewership?
* Which instructors are performing the best?

## 📊 Key Features & Insights

This one-page, fully interactive dashboard provides a 360-degree view of course performance:

* **📈 Category Performance:** A top-level slicer allows filtering the entire report by course category.
* **💡 Skills in Demand:** A **Word Cloud** visual (imported from AppSource) instantly highlights the most frequently mentioned skills in course-related data.
* **🏆 Category Ranking by Viewership:** A matrix powered by a **DAX measure** (`rank_category_by_avg_views`) identifies which categories are true high-performers, moving beyond simple counts to average engagement.
* **🔍 Drill-Down Analysis:** A column chart analyzes course popularity by language, with a **drill-down** feature to explore sub-categories within each language.
* **⌛ Engagement vs. Duration:** Two key line charts analyze viewer engagement:
    1.  Viewership based on the number of subtitles available.
    2.  Viewership based on the total duration (in hours) of the course, helping to find the "sweet spot" for content length.
* **⭐ Instructor Ratings:** A bar chart tracks average instructor ratings, making it easy to identify top-performing educators.
* **Overview Matrix:** A summary table provides a quick look at average skills, duration, and other key metrics by category.

## 🛠️ Technical Details

* **Tool:** Power BI Desktop
* **Data Source:** `Online_Courses.csv`
* **Data Transformation:** Power Query was used for data cleaning, handling null values, and ensuring correct data types.
* **Data Analysis:** DAX (Data Analysis Expressions) was used to create custom measures to provide deeper insights than the raw data allowed.
* **Visualization:** A strategic selection of visuals (bar, line, matrix, word cloud, slicers) was used to tell a clear and compelling story.

## 🚀 How to Use

1.  **Clone** or **download** this repository.
2.  Open the `EDTech DA.pbix` file in **Power BI Desktop**.
3.  Interact with the dashboard:
    * Select a category from the slicer at the top.
    * Hover over visuals to see detailed tooltips.
    * Right-click on the "Courses as per Language" chart and select "Drill Down" to see the sub-category data.
