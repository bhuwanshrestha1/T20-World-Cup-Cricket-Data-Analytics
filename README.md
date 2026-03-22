# 🏏 T20 World Cup Cricket Data Analytics Project

## 📋 Project Overview
This project entails a complete end-to-end data analytics and data engineering lifecycle using the T20 World Cup dataset. The primary objective of this project is to build a conceptual, data-driven "Best 11" cricket team utilizing various metrics and performance criteria derived from real match data.

## 🛠️ Tools & Technologies Used
- **Web Scraping:** JavaScript (Node.js/Bright Data) for data extraction.
- **Data Preprocessing & Cleaning:** Python, Pandas.
- **Data Visualization & Dashboarding:** Power BI.
- **Data Manipulation in Dashboard:** DAX (Data Analysis Expressions).
- **Development Tools:** Jupyter Notebook, Power BI Desktop.

## 🔄 Data Flow & Pipeline
1. **Web Scraping (JavaScript/Node.js)**
   - Extracted T20 World Cup data from ESPNCricinfo using web scraping scripts (`t20_wc_batting_summary.js`, `t20_wc_bowling_summary.js`, `t20_wc_match_results.js`, `t20_wc_player_info.js` located in `web_scrapping_codes/`).
   - The unstructured/semi-structured scraped data was stored in JSON format (`t20_json_files/`).

2. **Data Cleaning & Transformation (Python)**
   - Processed the raw JSON data using `t20_data_preprocessing.ipynb`.
   - Used the Pandas library to handle missing values, correct data types, format specific columns, merge necessary fields, and derive deeper analytical features.
   - The final, cleaned datasets were exported into CSV files (`t20_csv_files/`).

3. **Data Modeling & Dashboarding (Power BI)**
   - Loaded the clean CSV files into Power BI Desktop.
   - Established relationships across various tables (e.g., match results, batting summaries, bowling summaries, player info) to build a robust data model.
   - Formulated complex DAX measures (documented in `DAX-Measures-and-Calculated-Columns.xlsx`) such as:
     - **Batting Metrics:** Batting Average, Strike Rate, Boundary %.
     - **Bowling Metrics:** Bowling Average, Economy Rate, Dot Ball %.
   - Designed an interactive dashboard (`Cricket-Best-11.pbix`) with customized tooltips, filters, and slicers to evaluate players categorised into specific roles (Openers, Middle Order, Finishers, All-rounders, Specialist Bowlers).

## 📊 Dashboard Features
- **Player Performance Analysis:** Interactive visuals to dissect a player's performance against specific teams or in various match conditions.
- **Best 11 Selection Sandbox:** A specialized view permitting the dynamic filtering of players based on defined thresholds (e.g., minimum runs, minimum wickets, strike rate limits) to assemble the ultimate playing 11 purely heavily grounded in data.
-Screenshot:
<img width="1908" height="1073" alt="Dashboard" src="https://github.com/user-attachments/assets/018776f6-1ee3-46b1-8efa-2e8b0f28e0bc" />


## 🚀 How to Run or Reproduce the Project
1. Clone or download the repository.
2. *(Optional)* Run the JS files in the `web_scrapping_codes/` folder if you want to perform the scraping step yourself.
3. Open `t20_data_preprocessing.ipynb` in a Jupyter environment and execute the cells to generate the cleaned CSV outputs.
4. Open the `Cricket-Best-11.pbix` file using **Power BI Desktop** to explore the dashboard and visualizations.

## 🌟 Acknowledgements
This portfolio project was built following the Codebasics Data Analytics project series, implementing industry-standard practices for data extraction, transformation, visualization, and storytelling.
