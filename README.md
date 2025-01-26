# Docker Compose Demo Application

This project demonstrates a simple Docker Compose application with two containers:
1. **App Container**: A Python Flask web app.
2. **Redis Container**: A Redis instance used for caching data.

## **Project Structure**

```
.
├── app/
│   ├── app.py            # Python Flask application
│   ├── requirements.txt  # Dependencies for the app
│   ├── Dockerfile        # Dockerfile to containerize the app
├── docker-compose.yml    # Docker Compose file to orchestrate containers
└── README.md             # Project documentation
```

## **How to Build and Run**

### **1. Clone the Repository**
```bash
git clone https://github.com/Badal2456/docker-compose-demo.git
cd docker-compose-demo
```

### **2. Build and Start the Application**
```bash
docker-compose up --build
```

### **3. Access the Application**
Open your browser and navigate to:
```
http://localhost:5000
```

### **4. Stop the Application**
To stop all containers:
```bash
docker-compose down
```

## **Expected Output**
When you visit the app in your browser, you will see:
```
Hello from Docker Compose! This page has been visited X times.
```

## **Key Features**
- Demonstrates multi-container orchestration using Docker Compose.
- Uses Redis for caching and Flask for serving a simple web application.

## **Next Steps**
- Explore Docker Compose scaling with `docker-compose up --scale`.
- Extend the project to include persistent storage or additional services.
