# Virtual Travel Experience Explorer

The **Virtual Travel Experience Explorer** is an interactive data analytics project designed to help users explore and evaluate travel destinations. The project integrates multiple datasets such as destinations, weather, events, reviews, social media trends, and flight information. It demonstrates how to combine data ingestion, SQL-based querying, and interactive visualization to deliver actionable travel insights.

---

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Data Sources](#data-sources)
- [Technologies Used](#technologies-used)
- [Installation & Setup](#installation--setup)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Future Enhancements](#future-enhancements)
- [License](#license)

---

## Overview

The Virtual Travel Experience Explorer is designed to:
- **Integrate Multiple Data Sources:** Combine data from various travel-related CSV files.
- **Utilize SQL for Data Management:** Import CSV files into an SQLite database to enable robust querying and data integration.
- **Visualize Insights:** Use Python libraries (such as Pandas and Plotly) to create interactive visualizations that help users understand travel trends, weather conditions, event schedules, and flight details.
- **Serve as a Portfolio Project:** Demonstrate end-to-end data analysis skills—from data ingestion and transformation to visualization and SQL querying.

---

## Features

- **Data Ingestion & Integration:**  
  Import multiple CSV datasets into an SQLite database.

- **SQL Querying:**  
  Run SQL queries to join datasets, compute aggregates, and extract relevant insights.

- **Interactive Visualizations:**  
  Display travel data using interactive charts and graphs powered by Plotly.

- **Modular & Scalable Architecture:**  
  Designed to be extended into an industrial-grade application with additional features, APIs, and web-based dashboards.

---

## Data Sources

This project uses sample datasets that represent:
- **Destinations:** Information on travel destinations (city, country, region, description).
- **Weather:** Weather conditions (temperature, condition) corresponding to each destination.
- **Events:** Details about local events (event name, date, category).
- **Reviews:** User reviews and ratings for each destination.
- **Social Media Trends:** Social media mentions and sentiment scores related to destinations.
- **Flights:** Flight information including origin, price, duration, and departure dates.

*Note: You can replace these sample datasets with real-world data to further enhance the project.*

---

## Technologies Used

- **Python** for data processing and analysis.
- **Pandas** for data manipulation.
- **SQLite** (via Python's `sqlite3` module) for database management.
- **SQL** for querying and joining data.
- **Plotly** for interactive data visualizations.
- **Google Colab** for an interactive development environment (optional).
- **Google Drive** for data storage and file management (optional).

---

## Installation & Setup

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/virtual-travel-experience-explorer.git
   cd virtual-travel-experience-explorer
   ```

2. **Set Up Your Python Environment:**

   Create a virtual environment and install dependencies:

   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```

3. **Upload & Mount Data (For Google Colab Users):**

   - Upload your CSV files (destinations.csv, weather.csv, events.csv, reviews.csv, social_media.csv, flights.csv) to your Google Drive.
   - Mount your Drive in Colab:

     ```python
     from google.colab import drive
     drive.mount('/content/drive')
     ```

4. **Configure File Paths:**

   Update the file paths in the code to point to your CSV files in Google Drive if using Colab.

---

## Usage

1. **Data Loading & SQL Import:**

   Run the provided script to load CSV files into Pandas DataFrames and import them into an SQLite database.

2. **SQL Queries & Analysis:**

   Execute sample SQL queries to join tables and analyze data. The results are loaded back into Pandas for further processing and visualization.

3. **Visualization:**

   Use Plotly to create interactive charts (e.g., bar charts for temperature, pie charts for event categories, scatter plots for flight details).

4. **Run the Application:**

   If you have a web component or API, follow the instructions in the `main.py` or `api.py` modules to start the server.

---

## Project Structure

```
virtual-travel-experience-explorer/
│
├── README.md                  # This file
├── requirements.txt           # Python dependencies
├── destinations.csv           # Sample destination data
├── weather.csv                # Sample weather data
├── events.csv                 # Sample events data
├── reviews.csv                # Sample reviews data
├── social_media.csv           # Sample social media trends data
├── flights.csv                # Sample flights data
│
├── colab_notebook.ipynb       # Colab Notebook for running the project (optional)
├── main.py                    # Main entry point (for web/API integration)
├── etl.py                     # Module for ETL tasks (loading CSVs, validating data)
├── db.py                      # Database connection and models (using SQLite/SQLAlchemy)
├── api.py                     # Flask/FastAPI module for exposing endpoints (optional)
└── visualizations.py          # Module for creating interactive visualizations (optional)
```

---

## Future Enhancements

- **Database Upgrade:** Migrate from SQLite to PostgreSQL or MySQL for production-level performance.
- **API Development:** Develop a RESTful API for real-time data access and integration with front-end applications.
- **Dashboard Integration:** Build a web dashboard using frameworks like Dash or Streamlit for a more interactive user experience.
- **Data Ingestion Pipeline:** Implement an automated ETL pipeline using tools like Apache Airflow for scheduled data updates.
- **Containerization:** Use Docker to containerize the application for easier deployment and scalability.

---

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to contribute, raise issues, or suggest improvements. Enjoy exploring travel data and unlocking insights with the Virtual Travel Experience Explorer!

---

Created by Adnaan Khan and Vibhanshu Vaibhav
