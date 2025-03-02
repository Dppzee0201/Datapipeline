
# MCU End-To-End Data Pipeline

This project automates the process of collecting and organizing data about Marvel Cinematic Universe (MCU) films. It gathers movie and character details from Wikipedia, enriches the data with the OMDB API, and stores the cleaned dataset in an AWS S3 bucket in CSV format for further use.

## 🛠️ Features

- **Web Scraping**: Extracts MCU movie and character details using `Beautiful Soup` from Wikipedia.
- **Data Enrichment**: Fetches additional movie information using the `OMDB API`.
- **Serverless Processing**: Utilizes `AWS Lambda` for automated data extraction and transformation.
- **Data Lake Storage**: Stores the cleaned and transformed data as CSV files in an `AWS S3` bucket.
- **Data Transformation**: Cleans and organizes raw data into a structured format.


# Diagram

![Flow diagram](https://github.com/user-attachments/assets/b7746219-b268-4476-8f71-f46ea98d541e)``

## 🚀 How It Works

1. **Web Scraping**: Scrapes movie and character information from Wikipedia using Beautiful Soup.
2. **Data Enrichment**: Queries the OMDB API for additional movie metadata (e.g., IMDB ratings, release dates).
3. **Data Transformation**: Cleans and organizes the collected data for consistency.
4. **Data Storage**: Saves the transformed data in CSV format to an AWS S3 bucket.

## 🧰 Prerequisites

Ensure you have the following before starting:

- Python 3.10
- AWS Account (with access to S3 and Lambda)
- OMDB API Key

## 📊 Data Output

The output CSV files contain the following fields:

- Movie Title
- Release Date
- IMDB Rating
- Director
- Main Characters
- Box Office Collection
- 
## 📈 Future Improvements

- Add support for TV series in the MCU.
- Implement error handling and logging.
- Schedule Lambda functions using AWS EventBridge.

