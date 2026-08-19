# Consumer Attention System

An AI-powered retail analytics system that analyzes shopper behavior, attention, gaze, dwell time, shelf interaction, and product attractiveness to generate actionable recommendations.

---

## Project Overview

The **Consumer Attention System** uses Computer Vision and Artificial Intelligence techniques to understand how shoppers interact with products and shelves in a retail environment.

The system processes shopper activity and provides analytics through a web-based dashboard.

The platform combines:

- Shopper detection
- Shopper tracking
- Dwell-time analysis
- Shelf detection
- Gaze estimation
- Attention analysis
- Head-pose analysis
- Age and gender analysis
- Shopper behavior analysis
- Heatmap generation
- Product attractiveness scoring
- Product recommendations
- Dashboard analytics

---

## Key Features

- Shopper / person detection
- Shopper tracking with unique IDs
- Dwell-time analysis
- Shelf detection
- Gaze analysis
- Attention analysis
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

---

# System Architecture

```text
                    Consumer Attention System
                              |
             +----------------+----------------+
             |                                 |
          Frontend                           Backend
             |                                 |
        React + Vite                       FastAPI
             |                                 |
       Dashboard UI                    REST API Layer
                                             |
                         +-------------------+-------------------+
                         |                   |                   |
                    Computer Vision      Business Logic      Database
                         |                   |                   |
                    YOLO / ByteTrack     Services          PostgreSQL
                    InsightFace          Tracking
                    OpenCV              Analytics
                    Gaze Analysis       Recommendations




Technology Stack

Frontend
- React.js
- JavaScript (ES6+)
- HTML5
- CSS3
- Vite
- Axios
- React Router

Backend
- Python
- FastAPI
- Uvicorn
- SQLAlchemy
- Pydantic
- Alembic
- REST API

Database
- PostgreSQL

Artificial Intelligence & Computer Vision
- YOLOv8
- InsightFace
- OpenCV
- ByteTrack
- Computer Vision
- Face Detection
- Face Analysis
- Gaze Estimation
- Head Pose Estimation
- Attention Detection
- Shopper Tracking
- Dwell Time Analysis
- Behavioral Analysis

Machine Learning / AI Components
- Person Detection
- Face Detection
- Age & Gender Estimation
- Gaze Direction Estimation
- Geometric Attention Analysis
- Shopper Behavior Analysis
- Attention Confidence Scoring
- Product/Shelf Interaction Analysis
- Heatmap Generation

Development Tools
- Visual Studio Code
- Git
- GitHub
- Postman
- Python Virtual Environment
- Node.js
- npm

Project Architecture
- React.js Frontend
- FastAPI Backend
- PostgreSQL Database
- RESTful APIs
- AI/Computer Vision Processing Pipeline
- Alembic Database Migrations


Project Structure
---------------- 

Consumer_Attention_System/
│
├── Backend/
│   │
│   ├── app/
│   │   │
│   │   ├── api/
│   │   │   ├── analytics_routes.py
│   │   │   ├── auth.py
│   │   │   ├── dashboard_routes.py
│   │   │   ├── dwell_time_routes.py
│   │   │   ├── gateway.py
│   │   │   ├── heatmap_routes.py
│   │   │   ├── notification_routes.py
│   │   │   ├── product_score_routes.py
│   │   │   ├── shopper_behavior_routes.py
│   │   │   ├── store_routes.py
│   │   │   └── tracking_routes.py
│   │   │
│   │   ├── core/
│   │   │   ├── config.py
│   │   │   ├── database.py
│   │   │   └── security.py
│   │   │
│   │   ├── gaze/
│   │   │   ├── __init__.py
│   │   │   ├── attention_confidence.py
│   │   │   ├── attention.py
│   │   │   ├── face_analyzer.py
│   │   │   ├── gaze_estimator.py
│   │   │   ├── gaze_vector.py
│   │   │   ├── geometric_attention.py
│   │   │   ├── head_pose.py
│   │   │   ├── line_rectangle.py
│   │   │   ├── pose_smoother.py
│   │   │   ├── ray_intersection.py
│   │   │   ├── shelf_regions.py
│   │   │   └── utils.py
│   │   │
│   │   ├── middleware/
│   │   │   └── auth_middleware.py
│   │   │
│   │   ├── models/
│   │   │   ├── __init__.py
│   │   │   ├── interaction.py
│   │   │   ├── product_score.py
│   │   │   ├── role.py
│   │   │   ├── shelf.py
│   │   │   ├── shopper_attention.py
│   │   │   ├── shopper_behavior.py
│   │   │   ├── shopper_dwell_time.py
│   │   │   ├── shopper_tracking.py
│   │   │   ├── store.py
│   │   │   └── user.py
│   │   │
│   │   ├── schemas/
│   │   │   ├── auth.py
│   │   │   ├── interaction.py
│   │   │   ├── product_score.py
│   │   │   ├── shelf_schema.py
│   │   │   ├── shopper_attention.py
│   │   │   ├── shopper_behavior.py
│   │   │   ├── shopper_dwell_time.py
│   │   │   ├── shopper_tracking.py
│   │   │   └── store_schema.py
│   │   │
│   │   ├── services/
│   │   │   ├── analytics_service.py
│   │   │   ├── attention_service.py
│   │   │   ├── auth_service.py
│   │   │   ├── behavior_tracker.py
│   │   │   ├── dashboard_service.py
│   │   │   ├── detector.py
│   │   │   ├── dwell_time_service.py
│   │   │   ├── dwell_time_tracker.py
│   │   │   ├── heatmap_service.py
│   │   │   ├── notification_service.py
│   │   │   ├── product_score_service.py
│   │   │   ├── recommendation_service.py
│   │   │   ├── scoring_engine.py
│   │   │   ├── shelf_loader.py
│   │   │   ├── shelf_zone.py
│   │   │   ├── shopper_behavior_service.py
│   │   │   ├── tracker.py
│   │   │   ├── tracking_service.py
│   │   │   └── video_processor.py
│   │   │
│   │   └── utils/
│   │
│   ├── alembic/
│   │   ├── versions/
│   │   │   ├── 281dadd1a9f1_initial_tables.py
│   │   │   ├── 73181e0ce067_add_shelf_name_to_shopper_tracking.py
│   │   │   └── 8cee4f1e7509_add_product_scores.py
│   │   ├── env.py
│   │   ├── README
│   │   └── script.py.mako
│   │
│   ├── models_ai/
│   │   └── face_detection_yunet_2023mar.onnx
│   │
│   ├── tests/
│   │   └── test_recommendation_service.py
│   │
│   ├── trackers/
│   │   └── bytetrack.yaml
│   │
│   ├── heatmaps/
│   │
│   ├── alembic.ini
│   ├── main.py
│   ├── database.py
│   ├── requirements.txt
│   └── README.md
│
├── Frontend/
│   │
│   ├── public/
│   │   ├── favicon.svg
│   │   └── icons.svg
│   │
│   ├── src/
│   │   │
│   │   ├── assets/
│   │   │   ├── hero.png
│   │   │   ├── react.svg
│   │   │   └── vite.svg
│   │   │
│   │   ├── components/
│   │   │   ├── AttentionChart.jsx
│   │   │   ├── BehaviorTable.jsx
│   │   │   ├── DateCard.jsx
│   │   │   ├── HeatmapViewer.jsx
│   │   │   ├── Navbar.jsx
│   │   │   ├── ProtectedRoute.jsx
│   │   │   ├── QuickActions.jsx
│   │   │   ├── RecentActivity.jsx
│   │   │   ├── Sidebar.jsx
│   │   │   ├── StatCard.jsx
│   │   │   ├── SystemOverview.jsx
│   │   │   └── WelcomeCard.jsx
│   │   │
│   │   ├── pages/
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Login.jsx
│   │   │   └── Register.jsx
│   │   │
│   │   ├── services/
│   │   │   └── api.js
│   │   │
│   │   ├── styles/
│   │   │   ├── Auth.css
│   │   │   ├── behavior.css
│   │   │   ├── Cards.css
│   │   │   ├── Dashboard.css
│   │   │   ├── Footer.css
│   │   │   ├── Navbar.css
│   │   │   ├── Responsive.css
│   │   │   └── Sidebar.css
│   │   │
│   │   ├── App.css
│   │   ├── App.jsx
│   │   ├── index.css
│   │   └── main.jsx
│   │
│   ├── eslint.config.js
│   ├── index.html
│   ├── package-lock.json
│   ├── package.json
│   ├── README.md
│   └── vite.config.js
│
├── .gitignore
├── PPT.pptx
└── README.md
