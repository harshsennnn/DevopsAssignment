# Microservices Routing with Nginx and Health Checks

This project demonstrates:
- Two microservices (Go and Flask) exposing simple `/ping` and `/hello` endpoints
- Nginx reverse proxy for clean routing (`/service1/` and `/service2/`)
- Health checks to verify that the services are up before allowing traffic
- `docker-compose` setup for seamless orchestration

---
## Youtube Overview
[![IMAGE ALT TEXT HERE](https://img.youtube.com/vi/YOUTUBE_VIDEO_ID_HERE/0.jpg)](https://www.youtube.com/watch?v=-Uni6-EtNb4)
---
## 🧭 Setup Instructions

1. **Clone this repo**:


   ``bash
   git clone https://github.com/harshsennnn/DevopsAssignment.git
   cd DevopsAssignment``
   
3. **Run the services**:

   ``bash
  docker-compose up --build``

3. Test the endpoints:
    - Go: http://localhost/service1/ping , http://localhost/service1/hello
    - Flask: http://localhost/service2/ping , http://localhost/service2/hello

## 🐳 Features
- ✅ Nginx reverse proxy for unified routing
- ✅ Health check endpoints to ensure each service is live
- ✅ Go & Flask microservices containerized with Docker
- ✅ Easy one-command deployment with docker-compose

## ADD ON - Continuous Integration/Continuous Delivery Pipeline (Github Actions)

1. This GitHub Actions CI pipeline automatically builds and tests both the Go and Python microservices on every push or pull request. 

2. Builds the docker images and pushes them to docker hub 
