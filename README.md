# Airflow Implementation Using Weather Data API with Docker, PostgreSQL, and Astro

## 📌 Project Overview
This project focuses on building a **scalable and automated data pipeline** using **Apache Airflow** to fetch, process, and store weather data from an external API. The pipeline is containerized using **Docker**, stores data in **PostgreSQL**, and is orchestrated with **Astronomer (Astro)**.

## 🔥 Key Features
- **Automated Data Extraction**: Fetch real-time weather data from an external API.
- **Data Processing & Transformation**: Clean, transform, and structure the data.
- **Database Storage**: Store structured weather data in PostgreSQL for analysis.
- **Orchestration with Apache Airflow**: DAGs automate data ingestion and workflow execution.
- **Docker for Containerization**: Ensures isolated and scalable execution.
- **Monitoring with Astro**: Provides an intuitive UI for tracking DAG runs, failures, and logs.

## 🛠️ Tech Stack
- **Apache Airflow** (Orchestration)
- **Docker** (Containerization)
- **PostgreSQL** (Database)
- **Astronomer (Astro)** (Managed Airflow)
- **Weather Data API** (Data Source)

## 🚀 Setup and Installation
### 1️⃣ Clone the Repository
```sh
 git clone https://github.com/your-repo.git
 cd your-repo
```

### 2️⃣ Install Dependencies
Make sure you have **Docker** and **Astro CLI** installed.
```sh
 astro dev init  # Initialize Astro project
```

### 3️⃣ Start the Airflow Environment
```sh
 astro dev start  # Start Airflow locally with Docker
```

### 4️⃣ Configure Environment Variables
Create a `.env` file and add your API credentials:
```sh
 WEATHER_API_KEY=your_api_key
 POSTGRES_USER=your_username
 POSTGRES_PASSWORD=your_password
 POSTGRES_DB=weather_db
```

### 5️⃣ Deploy and Monitor DAGs
Access the Airflow UI at:
```
 http://localhost:8080
```
Enable and trigger DAGs from the UI to fetch and process weather data.

## 📊 Expected Workflow
1. **Airflow DAG** triggers the API request for weather data.
2. **Data Processing** cleans and structures the data.
3. **PostgreSQL Storage** stores the transformed data.
4. **Scheduled Runs** ensure periodic updates via Airflow.

## 🤝 Contributing
Feel free to submit issues, pull requests, or suggestions to enhance this project!

## 📜 License
This project is licensed under the MIT License.

---
🚀 **Built for scalable and automated weather data ingestion!**
