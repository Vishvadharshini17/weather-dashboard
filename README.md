# Delhi Weather Dashboard

A comprehensive backend project designed to process, store, and serve nearly 20 years of Delhi weather forecast data.

This system transforms raw CSV weather data into a structured format, stores it efficiently, and exposes RESTful APIs to retrieve and analyze weather insights such as temperature trends, humidity, pressure, and heat index.

## Project Objectives:
### Data Processing & Storage:

- Transform raw CSV data into a clean, structured format

- Handle missing or inconsistent data

- Normalize date/time fields for accurate querying

- Store processed data in an optimized data store

- Ensure modular and maintainable code architecture

## API Development:

- Build RESTful APIs for seamless data access

- Enable filtering by date and month

- Provide monthly statistical insights (High, Median, Minimum temperatures)

## Tech Stack:

### Database:

 - MySQL

### API Testing:

- Postman

### Other Tools:

- Git & GitHub

## Data Processing Workflow:

- Load CSV dataset

- Clean and validate data

- Convert date fields into standard datetime format

- Extract year and month for optimized querying

### Get Weather Details by Date:

GET

/weather/date/{yyyy-mm-dd}

### Response Includes:

- Weather Condition

- Temperature

- Humidity

- Pressure

### Get Weather Details by Month (Across 20 Years):

GET

/weather/month/{month}

Example:

/weather/month/07

Returns all July data across the 20-year dataset.

### Get Monthly Temperature Statistics for a Given Year:

GET

/weather/stats/{year}

Response Includes (For Each Month):

- Highest Temperature

- Median Temperature

- Minimum Temperature

### Sample API Response:
{
  "year": 2015,
  "month": "July",
  "highest_temp": 42.5,
  "median_temp": 36.8,
  "minimum_temp": 28.1
}

## Installation & Setup:

- Clone Repository
git clone https://github.com/your-username/delhi-weather-api.git
- Create Virtual Environment
python -m venv venv
- Install Dependencies
pip install -r requirements.txt
- Configure Database

### Server runs at:

http://localhost:8080

### Key Features:

- Efficient data normalization

- Optimized database indexing

- Clean modular codebase

## Challenges Addressed:

- Handling large historical datasets

- Date-time normalization

- Efficient query filtering

- Statistical computation (Median calculation)

## Future Enhancements:

- Add pagination for large queries

- Add caching layer (Redis)

- Deploy on AWS / Render

## Skills Demonstrated:

- Data Cleaning & Transformation

- Backend Development

- REST API Design

- Database Schema Design

## Author:

Vishvadharshini
