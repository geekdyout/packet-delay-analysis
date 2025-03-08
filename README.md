# Network Delay Analysis Tool

A modern web application for analyzing and visualizing network packet delays from various capture file formats (.pcap, .pcapng, .cap, .etl, .erf) using Flask, React, and Material UI.

## Project Structure
```
Hackenza_DelayAnalysis/
├── backend/           # Flask API and analysis code
├── frontend/         # React frontend with D3.js visualizations
├── docs/            # Project documentation
└── README.md        # This file
```

## Setup Instructions

### Backend Setup
1. Create and activate a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Unix/macOS
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Start the Flask server:
```bash
cd backend
python app.py
```

### Frontend Setup
1. Install Node.js dependencies:
```bash
cd frontend
npm install
```

2. Start the development server:
```bash
npm start
```

## Docker Setup
1. Build and run the backend:
```bash
docker build -t packet-analysis-backend ./backend
docker run -p 5000:5000 packet-analysis-backend
```

2. Build and run the frontend:
```bash
docker build -t packet-analysis-frontend ./frontend
docker run -p 3000:3000 packet-analysis-frontend
```

## Features
- Upload and analyze .pcapng files
- Calculate network delay metrics (latency, jitter, packet loss)
- Interactive visualizations using D3.js
- Protocol and IP-based filtering
- Optional PostgreSQL integration for persistent storage

## Testing
- Backend tests: `cd backend && pytest`
- Frontend tests: `cd frontend && npm test`

## API Documentation
- POST `/upload`: Upload .pcapng files
- GET `/analyze`: Retrieve analysis results

## License
MIT License
