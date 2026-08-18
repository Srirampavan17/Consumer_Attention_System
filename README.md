# Consumer Attention System

An AI-powered retail analytics system that analyzes shopper behavior, attention, gaze, dwell time, shelf interaction, and product attractiveness to generate actionable recommendations.

## Project Overview

The Consumer Attention System uses computer vision and AI techniques to understand how shoppers interact with products and shelves in a retail environment.

The system processes shopper activity and provides analytics through a web-based dashboard.

## Key Features

- Shopper/person detection
- Shopper tracking with unique IDs
- Dwell-time analysis
- Shelf detection
- Gaze and attention analysis
- Head-pose analysis
- Age and gender analysis
- Shopper behavior segmentation
- Heatmap generation
- Product attractiveness scoring
- Product recommendations
- Dashboard analytics
- Role-based dashboard APIs
- Notifications and alerts
- REST APIs using FastAPI
- PostgreSQL database integration
- React-based frontend

## Technology Stack

### Backend

- Python
- FastAPI
- SQLAlchemy
- PostgreSQL
- Uvicorn
- OpenCV
- YOLO
- ByteTrack
- InsightFace

### Frontend

- React
- Vite
- JavaScript
- Axios
- React Router
- Chart.js
- Recharts
- Lucide React

## Project Structure

```text
Consumer_Attention_System/
│
├── Backend/
│   ├── app/
│   │   ├── api/
│   │   ├── core/
│   │   ├── gaze/
│   │   ├── middleware/
│   │   ├── models/
│   │   ├── schemas/
│   │   ├── services/
│   │   └── utils/
│   ├── alembic/
│   ├── tests/
│   ├── trackers/
│   ├── models_ai/
│   ├── alembic.ini
│   └── ...
│
├── Frontend/
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── services/
│   │   └── styles/
│   ├── public/
│   ├── package.json
│   └── ...
│
├── .gitignore
└── README.md