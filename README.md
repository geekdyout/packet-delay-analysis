<<<<<<< HEAD
# Network Delay Analysis Tool

A modern web application for analyzing and visualizing network packet delays from various capture file formats (.pcap, .pcapng, .cap, .etl, .erf). The tool helps identify and troubleshoot network issues by analyzing latency, jitter, and packet loss patterns.

## Features
- Support for multiple packet capture formats (.pcap, .pcapng, .cap, .etl, .erf)
- Real-time packet analysis using Python/pyshark
- Interactive visualizations with React and Material UI
- RESTful API backend with Flask
- Modern, responsive user interface
- Comprehensive delay metrics calculation

## Project Structure
```
Hackenza_DelayAnalysis/
├── backend/           # Flask API and analysis code
├── frontend/         # React frontend with Material UI
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
=======
# packet-delay-analysis
Web-based tool analyzing .pcapng files for network delays. Uses Python/pyshark to compute latency, jitter, and packet loss. Visualizes results in an interactive React/D3.js dashboard with a Flask backend and  PostgreSQL persistence. Helps identify and troubleshoot network issues.
>>>>>>> origin/main
