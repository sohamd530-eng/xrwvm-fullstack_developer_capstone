# Dealerships Review Application - Full Stack Web Application
## IBM Full Stack Software Developer Capstone Project

A comprehensive full-stack responsive web application developed for **Cars Dealership**, a national car retailer in the United States. The platform enables prospective car buyers and dealership visitors to explore branch locations across the US, browse automotive makes and models, read verified customer reviews, analyze customer sentiment in real time, and submit authenticated dealership reviews.

---

## 🚀 Key Features

- **Dealership Locator**: Browse, search, and filter automotive dealerships across all 50 states (e.g., Kansas, California, Texas, New York).
- **Interactive Review System**: Read customer feedback for each dealership branch with sentiment analysis tags (Positive, Neutral, Negative).
- **Authentication & User Management**: Secure user registration, login, session management, and logout using Django authentication.
- **Car Inventory & Model Management**: Administrative dashboard to manage car manufacturers (CarMake) and corresponding vehicle models (CarModel) with SQLite persistence.
- **Microservices Architecture**:
  - **Node.js & MongoDB**: Microservice handling dealership directory and customer review database operations.
  - **Python Flask & NLTK**: Sentiment analysis microservice using `SentimentIntensityAnalyzer` to evaluate user feedback polarity.
- **Responsive User Interface**: Modern single-page frontend built with React, Bootstrap 5, and responsive CSS for desktop, tablet, and mobile displays.
- **CI/CD & Cloud Native Deployment**:
  - GitHub Actions automated testing and linting (`flake8`).
  - Containerized with Docker and orchestrated via Kubernetes.
  - Serverless container deployment on IBM Cloud Code Engine.

---

## 🛠️ Architecture & Tech Stack

| Layer | Technologies |
| :--- | :--- |
| **Frontend** | React.js, HTML5, CSS3, JavaScript (ES6+), Bootstrap 5 |
| **Primary Backend** | Django 4.2, Django REST Framework, Python 3.10, SQLite |
| **Dealership & Reviews DB** | Node.js, Express.js, MongoDB, Mongoose |
| **Sentiment Analysis** | Python Flask, NLTK SentimentIntensityAnalyzer |
| **Containers & Cloud** | Docker, Docker Compose, Kubernetes, IBM Cloud Code Engine |
| **CI/CD** | GitHub Actions |

---

## 📂 Project Structure

```
├── .github/
│   └── workflows/
│       └── main.yml           # GitHub Actions CI/CD Pipeline
├── screenshots/               # Project screenshots for Capstone submission tasks
├── server/
│   ├── database/              # Node.js + Express + MongoDB microservice
│   │   ├── app.js             # Mongoose API endpoints (/fetchDealers, /fetchReviews, etc.)
│   │   ├── dealership.js      # Dealership schema
│   │   ├── review.js          # Review schema
│   │   └── data/              # Initial seed datasets (dealerships.json, reviews.json)
│   ├── djangoapp/             # Django application backend
│   │   ├── models.py          # CarMake & CarModel ORM models
│   │   ├── views.py           # Authentication, dealer proxy, and review views
│   │   ├── restapis.py        # Microservice client helper methods
│   │   ├── urls.py            # Django application routing
│   │   ├── admin.py           # Admin interface configuration
│   │   ├── populate.py        # Database seed script for car models
│   │   └── microservices/     # Flask Sentiment Analysis microservice
│   │       └── app.py         # NLTK Sentiment Analysis endpoint (/analyze/<text>)
│   ├── djangoproj/            # Django project settings & root URLs
│   ├── frontend/              # React frontend application
│   │   ├── static/            # Static HTML views (Home.html, About.html, Contact.html)
│   │   └── src/               # React components (Register, Login, Dealers, Header)
│   ├── manage.py
│   └── requirements.txt
└── README.md
```

---

## ⚡ Quick Start Guide

### 1. Database Microservice (Node.js & MongoDB)
```bash
cd server/database
npm install
node app.js
# Runs on http://localhost:3030
```

### 2. Sentiment Analyzer Microservice (Flask)
```bash
cd server/djangoapp/microservices
pip install -r requirements.txt
python app.py
# Runs on http://localhost:5050
```

### 3. Django Web Server
```bash
cd server
pip install -r requirements.txt
python manage.py makemigrations
python manage.py migrate
python manage.py runserver 8000
# Runs on http://localhost:8000
```

---

## 👤 Author
- **Developer**: Soham ([@sohamd530-eng](https://github.com/sohamd530-eng))
- **Course**: IBM Full Stack Software Developer Professional Certificate (Capstone Project)