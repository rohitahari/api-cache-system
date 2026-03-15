## API Cache System

A backend system demonstrating cache-first architecture using FastAPI, Redis, and PostgreSQL.

This project shows how modern backend services improve performance by retrieving data from a cache before querying the database.


---

## Features

• Redis-based caching
• Database fallback
• Cache expiration
• Faster API responses
• Clean backend architecture


---

## Tech Stack

Python
FastAPI
Redis
PostgreSQL
SQLAlchemy
Uvicorn


---

## System Architecture

Client
   ↓
FastAPI API
   ↓
Redis Cache
   ↓
PostgreSQL Database

Flow:

Request received
↓
Check Redis cache
↓
If cached → return data
↓
If not cached → query database
↓
Store result in Redis
↓
Return response


---

## Project Structure

# api_cache_system
│
├── app
│   ├── main.py
│   ├── database.py
│   ├── models.py
│   ├── cache.py
│   ├── cache_service.py
│   └── routes.py
│
├── requirements.txt
└── README.md


---

## Run Locally

Install dependencies

pip install -r requirements.txt

Start Redis

redis-server

Run API

uvicorn app.main:app --reload --port 8004

Open documentation

http://127.0.0.1:8004/docs


---

## Example Request

GET /products/1

First response:

source: database

Second response:

source: cache


---

## Future Improvements

• Distributed caching
• Cache invalidation strategies
• API monitoring
• Cache analytics


---

Push to GitHub

Run inside the project folder:

git init
git add .
git commit -m "API Cache System with Redis and PostgreSQL"
git branch -M main
git remote add origin https://github.com/rohitahari/api-cache-system.git
git push -u origin main


---

Your Backend Portfolio Now

You now have 5 serious backend systems:

URL Shortener
Job Queue System
API Rate Limiter
Auth Service
API Cache System

These represent the core backend infrastructure patterns.

That means:

project-building phase → complete


---

If you want, the next thing I can show you is extremely important for the next stage:

the exact roadmap from these 5 projects → first $1000 online as a backend developer.
