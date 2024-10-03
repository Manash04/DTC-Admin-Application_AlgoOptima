Smart Urban Transit Management - A Smart Dynamic Bus Scheduling System
This repository contains the codebase for Smart Urban Transit Management, a project developed for the Smart India Hackathon 2024. The project is aimed at improving public transportation efficiency through smart scheduling, predictive maintenance, and AI-driven decision-making processes. The system leverages blockchain for crew payment, machine learning for route and crowd management, and dynamic scheduling for efficient bus allocation.

Repository Structure
The repository is organized into the following folders:

1. API
This folder contains the FastAPI-based backend used to handle various endpoints required for dynamic scheduling, crew management, and predictive maintenance.

Key features:

Dynamic scheduling API for adjusting bus frequencies based on real-time demand.
Predictive maintenance API for determining vehicle health based on key parameters.
Crew management API for tracking and managing crew schedules and payments.
2. Geocoding
This folder contains scripts that perform geocoding to obtain the latitude and longitude of bus stops. The geocoding process is essential for mapping out routes and determining bus stop locations.

Key features:

Geocoding of bus stops using address data.
Generation of bus stop coordinates for further analysis and mapping.
3. ML Model
This folder includes the machine learning models developed for various tasks in the project. The models are trained on a variety of datasets to provide insights and optimizations in different areas:

CarbonFootprintsTracking: Model to track and analyze the environmental impact of bus routes and vehicle emissions.
CrewManagement: AI-powered crew assignment and scheduling.
CrowdDetection: Model to detect crowd levels and dynamically adjust the frequency of buses based on real-time data.
DynamicScheduling: Predictive model to allocate bus routes based on demand patterns.
PredictiveMaintenance: Model for predicting the health and maintenance requirements of buses based on various factors such as engine health, tire pressure, fuel consumption, etc.
4. Web Application
This folder contains the frontend code for the web application, built using Next.js with Prisma as the ORM and TailwindCSS for styling. The web app provides a user-friendly interface for managing bus routes, schedules, and other services.

Key features:

User authentication with Metamask for crew payments.
Dashboard for live tracking, route management, and scheduling.
Crew and vehicle management using blockchain integration for transparency.
Real-time display of adjusted bus frequencies and vehicle health statistics.
Installation
Prerequisites
Python 3.9+
Node.js 16+
Docker (Optional, for containerized setup)
PostgreSQL (for database management via Prisma)
Aptos SDK for blockchain integration
Backend (FastAPI)
Navigate to the API folder and install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Run the FastAPI server:
bash
Copy code
uvicorn main:app --reload
Frontend (Next.js)
Navigate to the Web Application folder and install the required dependencies:
bash
Copy code
npm install
Run the Next.js development server:
bash
Copy code
npm run dev
Geocoding
Navigate to the Geocoding folder and install the required dependencies:
bash
Copy code
pip install -r requirements.txt
Run the geocoding script to generate latitude and longitude data:
bash
Copy code
python geocode.py
Machine Learning Models
Navigate to the ML Model folder and install dependencies for each model as specified in the corresponding requirements.txt files.
Train or run each model individually as per the model instructions.
Usage
Run the API: Start the FastAPI server to handle requests from the web application.
Run the frontend: Start the Next.js application to interact with the system.
Geocode bus stops: Use the geocoding scripts to process bus stop data.
Deploy ML models: Deploy the machine learning models to dynamically adjust bus schedules, predict maintenance, and manage crew.
Features
Dynamic Bus Scheduling: Adjusts bus frequencies based on real-time demand and data from past patterns.
Blockchain for Crew Payments: Crew members are paid using Aptos blockchain integration, ensuring transparency and security.
Predictive Maintenance: Predicts when a bus requires maintenance based on various parameters, reducing downtime.
Crowd Detection: Adjusts bus routes and schedules based on crowd density data.
Environmental Impact Tracking: Tracks and reduces the carbon footprint of the transportation system.
Crew Management: Efficient scheduling of crew members using AI-driven optimization techniques.
License
This project is licensed under the MIT License - see the LICENSE file for details.

