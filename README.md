Distributed URL Shortener
A scalable distributed URL shortening platform inspired by Bitly and TinyURL.
This project demonstrates modern software engineering and system-design concepts including API design, distributed caching, analytics tracking, database indexing, scalable backend architecture, and containerized deployment.

🚀 Features


Convert long URLs into short URLs


Custom short aliases


URL redirection


Click analytics tracking


RESTful APIs


Scalable backend architecture


Dockerized deployment


Analytics-ready system design


Redis-ready caching architecture


High-performance URL lookup



🧠 System Design Concepts
This project demonstrates:


Distributed systems architecture


API Gateway concepts


Load balancing


Caching strategies


Database indexing


Analytics pipelines


Horizontal scaling


Stateless service design


Docker containerization



🛠️ Tech Stack
Frontend


React


Vite


CSS


Backend


Python


FastAPI


Database


SQLite (Local)


PostgreSQL Ready


Future Scale Components


Redis


Kafka


Kubernetes


Deployment


Docker


Docker Compose



🏗️ Architecture Diagram
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/4fc39d5e-77f9-4ecb-8448-f0e2b0e77396" />


🔥 Workflow Diagram
<img width="1536" height="1024" alt="image" src="https://github.com/user-attachments/assets/00ffcf6e-a03b-4909-a7f5-df16bc0cac06" />


📁 Project Structure
distributed-url-shortener/
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   ├── database.py
│   │   ├── models.py
│   │   └── schemas.py
│   │
│   ├── requirements.txt
│   └── Dockerfile
│
├── frontend/
│   ├── src/
│   │   ├── App.jsx
│   │   └── style.css
│   │
│   ├── package.json
│   └── index.html
│
├── screenshots/
│   ├── architecture.png
│   └── workflow.png
│
├── docker-compose.yml
└── README.md

⚙️ Backend Setup
Create virtual environment
python -m venv venv
Activate environment
Windows
venv\\Scripts\\activate
Linux/Mac
source venv/bin/activate

📦 Install Dependencies
pip install -r requirements.txt

▶️ Run Backend
uvicorn app.main:app --reload
Backend runs at:
http://localhost:8000
Swagger Docs:
http://localhost:8000/docs

▶️ Run Frontend
npm installnpm run dev
Frontend runs at:
http://localhost:5173

🐳 Docker Setup
Run complete project:
docker-compose up --build

📌 API Endpoints
Create Short URL
POST /api/shorten
Request
{  "original_url": "https://example.com",  "custom_code": "demo"}
Response
{  "short_code": "demo",  "short_url": "http://localhost:8000/demo",  "original_url": "https://example.com"}

Redirect URL
GET /{short_code}

Get Analytics
GET /api/stats/{short_code}

📊 Example Analytics Response
{  "short_code": "demo",  "original_url": "https://example.com",  "clicks": 42,  "created_at": "2026-05-08T12:00:00"}

💼 Portfolio Description
Built a scalable distributed URL shortener platform using FastAPI and React with support for short link generation, custom aliases, redirects, and click analytics. Designed the architecture using distributed systems principles including caching, indexing, API-driven services, and horizontally scalable deployment strategies.

💼 Resume Bullets


Developed a distributed URL shortening platform using FastAPI, React, and SQL-based storage with support for redirects, analytics tracking, and custom aliases.


Designed scalable backend APIs and analytics workflows demonstrating distributed systems concepts including caching, indexing, and stateless service architecture.


Containerized frontend and backend services using Docker Compose and documented future scalability enhancements using Redis, Kafka, and Kubernetes.



🔮 Future Improvements


Redis distributed caching


Kafka analytics pipeline


PostgreSQL production deployment


Rate limiting


QR code generation


Kubernetes deployment


User authentication


Dashboard analytics


Multi-region deployment



🧪 Example System Design Extensions
This architecture can be extended with:


Redis for ultra-fast URL lookups


Kafka for event streaming


PostgreSQL sharding


Load balancers


CDN edge caching


Kubernetes orchestration


Distributed analytics processing



👨‍💻 Author
Nivas Ramagiri
