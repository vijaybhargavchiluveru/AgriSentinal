#  AgriSentinal
> *See Beyond the Surface. Heal the Root.*

AI-powered crop health platform that detects disease, pests, and soil stress **before visible damage occurs** — using spectral imaging, IoT sensors, and deep learning.

---

## Problem
Farmers lose billions annually because crop diseases, pest attacks, and soil issues go undetected until it's too late. **500M+ smallholder farmers** have zero access to precision agriculture tools.

##  Solution
Root Cause ingests drone/satellite imagery + soil sensor data → runs AI analysis → delivers actionable recommendations to farmers in real time.

---

##  How It Works

```
Drone / Satellite Image + IoT Sensors
           ↓
   Image Processing (NDVI, Band Analysis)
           ↓
  AI Models: CNN (Crop Health) · YOLOv8 (Pests) · XGBoost (Soil)
           ↓
     FastAPI Backend + PostgreSQL
           ↓
  React Dashboard → Farmer Recommendations
```

**NDVI Formula:**
```
NDVI = (NIR − RED) / (NIR + RED)   →   High = Healthy · Low = Stressed
```

---

##  Tech Stack

| Layer | Tools |
|---|---|
| AI / ML | Python, TensorFlow, PyTorch, OpenCV, Rasterio |
| Backend | FastAPI, PostgreSQL, MongoDB |
| Frontend | React.js, Tailwind CSS, Leaflet.js |
| Cloud | AWS / GCP, Docker, GitHub Actions |
| Satellite | Sentinel-2, NASA EarthData |

---

##  API Endpoints

```
POST  /upload-image          → Upload farm image for analysis
GET   /crop-health/{farm_id} → AI crop health report
GET   /pest-risk/{farm_id}   → Pest detection + risk level
GET   /soil-status/{farm_id} → Soil condition analysis
GET   /recommendations/{id}  → Irrigation & fertilizer advice
```

---

##  Project Structure

```
root-cause/
├── ai-model/      # CNN, YOLOv8, XGBoost training
├── backend/       # FastAPI app + DB models
├── frontend/      # React dashboard + maps
├── datasets/      # Raw & processed imagery
└── documentation/
```

---

##  Team

| Member | Role |
|---|---|
|  Vijay | AI / Machine Learning |
|  Srinivas | Backend APIs |
|  Aarif | Frontend Dashboard |
|  Jayavardhan | Data Integration & Presentation |

---

##  Quick Start

```bash
git clone https://github.com/vijaybhargavchiluveru/root-cause.git

# Backend
cd backend && pip install -r requirements.txt && uvicorn main:app --reload

# Frontend
cd frontend && npm install && npm run dev
```

---

<p align="center"><em>Built by · Vijay · Srinivas · Aarif · Jayavardhan</em></p>
