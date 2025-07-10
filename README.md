# ETL-Pipeline: Largest Banks Market Capitalization
This project is an end-to-end ETL (Extract, Transform, Load) pipeline that retrieves data from Wikipedia about the largest banks in the world by market capitalization, transforms the data using currency exchange rates, and loads it into both a CSV file and an SQLite database.

## 🔧 Technologies Used

- Python 3
- pandas
- numpy
- requests
- BeautifulSoup (bs4)
- SQLite (via sqlite3)

## 🚀 Features

- Extracts a table from a static archived version of Wikipedia
- Cleans and parses market capitalization data
- Converts market cap values from USD to GBP, EUR, and INR using custom exchange rates
- Saves the transformed data to:
  - A local CSV file
  - A local SQLite database (`Banks.db`)
- Logs all steps and events to a log file (`code_log.txt`)
- Includes a sample SQL query to validate stored data

## 📦 File Structure

├── etl-largest-banks-market-cap.ipynb # Main Python script
├── exchange_rate_data.ipynb # Create exchange_rate.csv
├── exchange_rate.csv # Currency conversion rates
├── transformed_data.csv # Output file with converted values
├── Banks.db # SQLite database (created after first run)
└── code_log.txt # Log file generated during execution


## 📝 Prerequisites

Install required packages using pip:

```bash
pip install pandas numpy requests beautifulsoup4

## 📌 Notes
The Wikipedia URL used is an archived version for consistency.

The exchange rate file is simplified for demonstration. In real-world scenarios, dynamic FX API integration is recommended.

## 👤 Author
Hung Nguyen

GitHub link: https://github.com/hungnguyen820

Email: hungnguyen29820@gmail.com
