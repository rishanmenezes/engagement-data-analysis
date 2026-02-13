PROJECT TITLE
- Website Traffic and Engagement Analysis

PROJECT OVERVIEW
- This project performs an Exploratory Data Analysis (EDA) on website traffic data to evaluate user engagement and channel performance. By analyzing metrics such as sessions, users, and engagement rates across different marketing channels (e.g., Organic Social, Direct), the project aims to uncover trends in user behavior and identify the most effective sources of high-quality traffic.

DATASET DESCRIPTION
The dataset ("data-export.csv") contains 3,182 records of web analytics data with the following key columns:
1. Channel Group: The primary marketing channel (e.g., Direct, Organic Social).
2. DateHour: The timestamp of the session data (YYYYMMDDHH format).
3. Users: The number of unique visitors.
4. Sessions: The total number of visits.
5. Engaged Sessions: Visits that lasted longer than a threshold or involved key interactions.
6. Avg Engagement Time: Average time a user spent engaged during a session.
7. Engagement Rate: The percentage of sessions that were engaged.
8. Event Count: Total number of user interactions (events) recorded.

OBJECTIVES OF THE PROJECT
- To process and clean raw web analytics data for analysis.
- To visualize traffic trends over time (hourly and daily).
- To compare the performance of different traffic channels in terms of user volume and engagement quality.
- To analyze the relationship between session volume and engagement rates.
- To identify peak hours for user activity.

STEPS PERFORMED
1. Data Loading: Imported the CSV data using Pandas and handled the header structure.
2. Data Cleaning:
   - Renamed columns for clarity (e.g., "Session primary channel group" to "Channel Group").
   - Converted the "DateHour" string column into a usable datetime object.
   - Coerced numeric columns to ensuring correct data types for calculation.
3. Feature Engineering:
   - Extracted the "Hour" from the timestamp to allow for hourly traffic analysis.
4. Data Visualization:
   - Plotted time-series graphs to show the fluctuation of sessions and users over time.
   - Created bar charts to compare "Average Engagement Time" and "Engagement Percentage" across different channels.
   - Generated a scatter plot to analyze the correlation between total sessions and engagement rate.
   - Visualized hourly traffic patterns for each channel group.
5. Insight Generation: Identified which channels drive the most engaged users and when traffic peaks occur.

TOOLS AND LIBRARIES USED
- Python
- Pandas (for data manipulation and time-series handling)
- NumPy (for numerical operations)
- Matplotlib & Seaborn (for data visualization)
- Jupyter Notebook

FILES INCLUDED
- Data_export.ipynb: The Jupyter Notebook containing the code for data cleaning, analysis, and plotting.
- data-export.csv: The raw analytics dataset used for the project.

HOW TO RUN THE PROJECT
1. Install the required libraries:
   pip install pandas numpy matplotlib seaborn
2. Download "Data_export.ipynb" and "data-export.csv" to the same directory.
3. Open the notebook in Jupyter Notebook or VS Code.
4. Run the cells sequentially to reproduce the cleaning steps and visualizations.

KEY INSIGHTS
- Channel Performance: Different channels show distinct behaviors; for example, "Direct" and "Organic Social" appear to be significant drivers of traffic.
- Engagement Quality: Not all high-traffic channels lead to high engagement. The analysis highlights which channels bring users who actually stay and interact.
- Temporal Trends: User activity fluctuates significantly by hour, allowing for optimized timing of content or campaigns.
- Correlation: The scatter analysis helps determine if higher traffic volume necessarily correlates with better or worse engagement rates.

CONCLUSION
- This analysis provides a comprehensive view of website performance. By understanding which channels drive the most valuable (engaged) users and identifying peak activity times, stakeholders can optimize their digital marketing strategies to improve overall ROI and user retention.

AUTHOR
- Rishan Menezes
