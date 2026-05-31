⚽ Football Analytics Dashboard – PySpark & Power BI
📌 Project Overview

Football data provides valuable insights into team performance, seasonal trends, and competitive dynamics. This project aims to build a complete analytics pipeline using PySpark to process Bundesliga football match data and Power BI to create interactive dashboards.

The pipeline starts with loading and preparing raw CSV data, followed by data cleaning and transformation. Advanced performance indicators are then calculated for each team and season, allowing the identification of league champions and the evaluation of team performance through key metrics such as win percentage, goals scored, goals conceded, and goal differential.

Processed data is stored in optimized Parquet format and used to power a dynamic Power BI dashboard that enables users to explore football statistics across multiple seasons.

🎯 Project Objectives

The objective of this project is to transform raw football match data into meaningful insights through a modern data engineering and business intelligence workflow. Using PySpark, the project calculates team performance statistics, ranks teams within each season, identifies champions, and generates datasets optimized for analytical reporting. The final step consists of creating an interactive Power BI dashboard that allows users to analyze football performance from different perspectives.

🛠 Technologies Used

This project was developed using PySpark for data processing and transformation, Google Colab as the development environment, Parquet as the storage format, Matplotlib for exploratory visualizations, and Power BI Desktop for dashboard creation. GitHub was used for version control and project documentation.

🔄 Data Processing Pipeline

The project begins with importing football match data from a CSV file into a PySpark DataFrame. After understanding the dataset structure, unnecessary columns are removed and data types are verified to ensure consistency throughout the pipeline.

Additional columns are created to classify match outcomes. These indicators make it possible to distinguish home wins, away wins, and draws, simplifying future calculations and aggregations.

The dataset is then filtered to retain only Bundesliga matches and seasons between 2000 and 2015. This ensures that all analyses focus on a consistent competition and time period.

Team performance statistics are calculated separately for home matches and away matches. These results are merged to create a comprehensive dataset containing all team performance metrics for each season.

Advanced indicators are subsequently generated, including total wins, losses, draws, goals scored, goals conceded, goal differential, goals per game, goals against per game, and win percentage. These metrics provide a complete view of team performance.

To determine rankings, Spark Window Functions are used to compare teams within the same season. Teams are ordered according to their win percentage and goal differential, producing a final seasonal ranking and identifying the champion team.

Finally, the processed datasets are exported in Parquet format. One dataset contains all teams and their statistics, while another contains only the champions of each season.

📊 Power BI Dashboard

The Power BI dashboard was developed to provide an intuitive and interactive experience for exploring football statistics. It includes a set of key performance indicators that summarize the overall results of the league and highlight the most important trends.

Users can analyze total goals scored, total wins, average win percentage, and the number of participating teams. Interactive filters allow exploration by season, team, and team position, making the dashboard flexible and user-friendly.

Several visualizations have been created to compare team performances, track win percentages across seasons, analyze home and away results, and understand how team rankings evolve over time. These visual insights help transform complex football data into easily understandable information.

💾 Data Storage

The final datasets are stored in Parquet format to improve storage efficiency and query performance. The main dataset is partitioned by season, allowing faster access and better scalability when working with large volumes of football data. A separate dataset containing only season champions is also generated to support focused analyses on winning teams.

📈 Business Value

This project demonstrates how sports data can be transformed into actionable insights through data engineering and business intelligence techniques. Analysts can evaluate team performance over multiple seasons, supporters can easily identify league champions, and sports managers can use performance indicators to support strategic decision-making. The combination of PySpark and Power BI provides a scalable solution capable of handling large datasets while delivering clear and interactive visualizations.

🚀 Conclusion

This project successfully combines Big Data processing and Business Intelligence to create a complete football analytics solution. From raw CSV data to interactive dashboards, the entire workflow demonstrates how modern data technologies can be used to analyze sports performance, identify champions, and generate valuable insights from historical football data.

<img width="1165" height="654" alt="Screenshot (1657)" src="https://github.com/user-attachments/assets/9d621000-6799-4c97-bbcc-12794d2a209a" />

