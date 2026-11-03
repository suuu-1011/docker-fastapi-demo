Dockerized FastAPI Demo

A simple REST API built using FastAPI and Docker. This project provides a health-check endpoint to verify that the API service is running.

## Tech Stack
- Python 3.11
- FastAPI
- Uvicorn
- Docker
- Docker Compose

## Project Structure
docker-fastapi-ddemo/
├── app/
│ └── main.py
├── screenshots/
│ └── health-check.png
├── Dockerfile
├── docker-compose.yml
├── requirements.txt
└── README.md

## API Endpoint

| Method | Endpoint | Description |
| GET | `/health` | Checks API health |

### Expected Response
{
  "status": "ok"
}

## How to Run

### Prerequisite
Install and start Docker Desktop.

### Start the application

Open a terminal in the project directory and run:

docker compose up --build

The API will be available at:

http://localhost:8000

### Test the health endpoint

Open:

http://localhost:8000/health

Or send a GET request using Postman.

### Stop the application

Press `Ctrl + C` in the terminal, then run:

docker compose down


## Postman Screenshot

![Postman Health Check](screenshots/health-check.png)