# END-TO-END-YOUTUBE-DATA-PIPELINE

## 📌 Project Overview

This project simulates a modern Data Engineering pipeline that extracts,
processes, and analyzes data from the YouTube Data API v3.\
The pipeline follows an **ETL (Extract, Transform, Load)** architecture
and ends with data visualization in Power BI.

------------------------------------------------------------------------

## 🎯 Objectives

-   Extract data from a REST API (YouTube Data API v3)
-   Handle pagination and API limitations
-   Build a robust data ingestion process
-   Secure API credentials using environment variables
-   Transform raw JSON data into a structured dataset
-   Analyze and visualize data using Power BI

------------------------------------------------------------------------

## 🧱 Pipeline Architecture

YouTube API → Python Ingestion → Raw Storage (JSON) → Transformation →
Structured Dataset → Power BI

------------------------------------------------------------------------

## 🪜 Project Steps

### 1. Environment Setup

-   Create Python virtual environment
-   Install dependencies (requests, pandas, dotenv)
-   Organize project structure

### 2. API Configuration

-   Create Google Cloud project
-   Enable YouTube Data API v3
-   Generate API key
-   Understand quotas and pagination

### 3. Security

-   Store API key in `.env`
-   Load environment variables securely
-   Follow best practices to avoid exposing credentials

### 4. Data Extraction (Channel)

-   Retrieve channel data
-   Identify playlists and uploads

### 5. Extract Video IDs

-   Use PlaylistItems endpoint
-   Handle pagination
-   Collect all video IDs

### 6. Extract Video Details

-   Batch requests using Videos endpoint
-   Extract:
    -   Title
    -   Publish date
    -   Duration
    -   Views, likes, comments

### 7. Data Transformation

-   Convert JSON → tabular format
-   Clean and normalize data
-   Handle missing values

### 8. Data Storage

-   Save dataset (CSV/JSON)
-   Maintain structured data folders

### 9. Data Visualization

-   Import into Power BI
-   Build dashboards:
    -   Video performance
    -   Engagement metrics
    -   Trends over time

------------------------------------------------------------------------


## 🚀 Bonus Features

### 🐳 Docker

-   Containerize the pipeline
-   Ensure portability

### 🔁 Airflow

-   Automate ETL workflow
-   Schedule pipeline execution

### 🧠 Improvements

-   Add database (PostgreSQL / SQL Server)
-   Use data warehouse
-   Implement monitoring

------------------------------------------------------------------------

## 🛠️ Tech Stack

-   Python
-   YouTube Data API v3
-   Pandas
-   Power BI
-   Docker (optional)
-   Airflow (optional)

------------------------------------------------------------------------

## 📂 Project Structure

    project/
    │── data/
    │   ├── raw/
    │   ├── processed/
    │── src/
    │── config/
    │── .env
    │── requirements.txt
    │── README.md

------------------------------------------------------------------------

## 📊 Output

A clean analytical dataset ready for business intelligence and
dashboarding.

------------------------------------------------------------------------

## 👨‍💻 Abdelali Ouhsine

Data Engineering Project
