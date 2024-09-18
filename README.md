# Amazon Stock Data Scraping Project

This project is focused on scraping historical stock data for Amazon from a given webpage using Python. The data is collected from a simulated Yahoo Finance page and stored in a structured format using the `pandas` library. This project is intended to demonstrate web scraping techniques with `BeautifulSoup` and data manipulation using `pandas`.

## Project Overview

The goal of this project is to scrape Amazon's historical stock data, including the following fields:
- **Date**
- **Open Price**
- **High Price**
- **Low Price**
- **Close Price**
- **Adjusted Close Price**
- **Volume**

The scraped data is then loaded into a `pandas` DataFrame for further analysis.

## Tools and Libraries Used

- **Python 3.x**: Programming language used for the project.
- **pandas**: Library for data manipulation and analysis.
- **requests**: Library for making HTTP requests to fetch webpage data.
- **BeautifulSoup**: Library from `bs4` for parsing HTML and scraping data from the web.

## How It Works

1. **Fetching the Webpage**: The `requests` library is used to retrieve the webpage containing the stock data.
2. **Parsing HTML**: Using `BeautifulSoup`, the HTML content is parsed to extract the relevant table containing Amazon's historical stock data.
3. **Extracting Data**: The stock data for each date is extracted and stored in a `pandas` DataFrame, with columns representing Date, Open, High, Low, Close, Adjusted Close, and Volume.
4. **DataFrame Creation**: The extracted data is concatenated into the `amazon_data` DataFrame, ready for further analysis or exporting.
