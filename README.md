# ClimateIQ — Python Mini Project

### Climate Intelligence for Heatwave Monitoring, Prediction and Early Warning

**Academic Year:** 2026–2027  
**Department:** Information Technology  
**Institution:** K. J. Somaiya School of Engineering, Somaiya Vidyavihar University  
**Subject:** Object-Oriented Programming using Python  
**Project Type:** Python Mini Project

## 1. Project Overview

ClimateIQ is a web-based heatwave monitoring and early-warning system developed to display and analyze climate conditions across selected regions of Maharashtra.

The application uses **Python Flask** as its backend framework to retrieve climate information from a PostgreSQL database and provide it to a React frontend through a REST API.

Users can select different regions, view temperature and heat index information, examine heatwave risk levels, and explore graphical weather summaries.

The current implementation uses illustrative climate data for demonstration purposes.

## 2. Problem Statement

Extreme heat conditions can affect public health, infrastructure and daily activities. Climate information is often difficult to interpret when weather readings, forecasts and warnings are presented separately.

ClimateIQ aims to organize relevant climate information and present it through an interactive dashboard, making regional heatwave conditions easier to understand.

## 3. Project Objectives

- Develop a Python-based backend using Flask.
- Retrieve climate information from a PostgreSQL database.
- Implement REST API communication using JSON.
- Display regional weather conditions and heatwave risk indicators.
- Visualize climate parameters through interactive charts.
- Demonstrate Python modules, functions, database connectivity and error handling.
- Deploy the application for browser-based access.

## 4. Technology Stack

| Technology | Purpose |
|---|---|
| Python | Backend programming language |
| Flask | REST API and request handling |
| python-dotenv | Loading environment configuration |
| PostgreSQL | Relational data storage |
| React + Vite | Interactive frontend |
| JavaScript / JSX / CSS | Frontend logic and styling |
| Recharts | Graphical climate visualization |
| Git and GitHub | Version control and source-code hosting |
| Render | Backend deployment |
| Neon | Cloud PostgreSQL hosting |
| Vercel | Frontend deployment |

**Note:** The exact PostgreSQL Python driver and remaining backend dependencies should be checked against `backend/requirements.txt` before final submission.

## 5. Python Concepts Used

### Python Modules

The backend is organized into separate Python files to improve code organization and maintainability.

- `backend/app.py` — Flask application and API logic.
- `backend/database.py` — PostgreSQL database connection and data retrieval logic.

### Python Functions

Functions are used to organize backend operations, including request processing and database access.

### Flask Framework

Flask handles incoming HTTP requests and sends responses to the frontend.

The main dashboard API endpoint is:

`GET /dashboard`

### JSON Handling

Climate data retrieved through the backend is returned in JSON format so the React application can process and display it.

### Database Connectivity

Python connects to PostgreSQL to retrieve records needed for the dashboard.

Database connection settings are managed through environment configuration rather than hardcoded credentials.

### Error Handling

Backend and frontend error handling help identify database connection problems, unsuccessful requests and unavailable API responses.

### Python Virtual Environment

A Python virtual environment (`.venv`) is used during development to manage project dependencies separately from the system Python installation.

## 6. System Architecture

The application follows a three-tier architecture:

**Frontend (React + Vite)**  
↓ HTTP request  
**Backend (Python Flask)**  
↓ SQL queries  
**Database (PostgreSQL)**  
↓ Query results  
**Flask JSON response**  
↓  
**React dashboard visualization**

The frontend is deployed on Vercel, the Flask backend on Render, and the PostgreSQL database on Neon.

## 7. Application Workflow

1. The user opens the ClimateIQ website.
2. The React frontend requests dashboard data from Flask.
3. Flask communicates with PostgreSQL.
4. The required climate information is retrieved.
5. The backend returns a JSON response.
6. React processes the response and updates the interface.
7. The user can switch between regions and examine weather metrics, charts and risk information.

## 8. Main Features

- Interactive dashboard for 10 Maharashtra regions.
- Region-wise temperature and heat index display.
- Humidity, wind speed, pressure and cloud-cover information.
- Heatwave risk and alert-level indicators.
- Graphical representation of climate metrics.
- Stakeholder information panel.
- Loading and error states for API requests.
- Deployed frontend and backend.

## 9. Project Structure

Key files and directories include:

```text
climateiq-python-mini-project/
├── backend/
│   ├── app.py
│   ├── database.py
│   └── ...
├── src/
│   └── App.jsx
├── package.json
├── README.md
└── ...
```

This is a simplified structure showing the main application files.

## 10. Running the Project Locally

### Backend

Open the backend folder and activate the project's Python virtual environment.

Install the backend dependencies from the project's requirements file, where provided:

```bash
pip install -r requirements.txt
```

Start the Flask application:

```bash
python app.py
```

The local Flask server typically runs at:

`http://127.0.0.1:5000`

A valid database configuration is required.

### Frontend

Open the frontend project folder and run:

```bash
npm install
npm run dev
```

Open:

`http://localhost:5173`

The frontend must be configured to communicate with the correct backend URL.

## 11. Results

The deployed ClimateIQ application was tested for:

- Successful dashboard loading.
- Display of 10 regions.
- Region selection and interface updates.
- Climate charts, alerts and stakeholder information.
- Successful page refresh.

These tests demonstrate the integration of Python Flask, PostgreSQL and React.

## 12. Limitations

- Climate readings are illustrative demonstration data rather than live sensor observations.
- A trained and independently validated machine-learning prediction model has not been implemented.
- Some advanced data-management features remain future enhancements.

## 13. Future Scope

- Integration with real weather APIs and sensor networks.
- Development of a trained machine-learning model.
- Historical climate trend analysis.
- Authenticated administrative data management.
- Expanded alert-delivery functionality.
- Improved backend testing and monitoring.

## 14. Live Application

**Frontend:** https://climate-intelligence-mauve.vercel.app/

**Backend API:** https://climateiq-backend.onrender.com/dashboard

## 15. GitHub Repository

https://github.com/deshna1903/climateiq-python-mini-project

## 16. References

- Python Documentation — https://docs.python.org/3/
- Flask Documentation — https://flask.palletsprojects.com/
- PostgreSQL Documentation — https://www.postgresql.org/docs/
- React Documentation — https://react.dev/
- Vite Documentation — https://vite.dev/
- Recharts Documentation — https://recharts.org/

---

**Developed as a Python Mini Project for Academic Year 2026–2027.**