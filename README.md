# Cloud Record Storage API (cloud-record-storage-api)

A secure and scalable API for storing and retrieving JSON records in the cloud. Built with NestJS (TypeScript), this service provides robust authentication (OAuth 2.0) and efficient data management with Redis caching and PostgreSQL persistence.

Key Features:

* **Secure Record CRUD:** RESTful API endpoints for creating, reading, updating, and deleting JSON records.
* **OAuth 2.0 Authentication:** Robust user authentication and authorization using OAuth 2.0.
* **Redis Cache-Aside:** Optimized performance with Redis caching for frequently accessed data.
* **PostgreSQL Persistence:** Reliable data storage using PostgreSQL.
* **Race Condition Protection:** Implemented database transactions to ensure data integrity.
* **Microservices Architecture:** Designed for scalability and maintainability.

Infrastructure & Deployment:

* **Infrastructure as Code (Terraform):** Cloud resources (GKE, Cloud SQL, Memorystore) are provisioned and managed using Terraform.
* **Containerization (Docker):** The NestJS API is containerized using Docker for consistent deployment.
* **Kubernetes Orchestration (GKE):** Docker containers are orchestrated using Google Kubernetes Engine (GKE) for scalability and resilience.
* **Service Mesh (Istio):** Istio is used for traffic management, security, and observability within the Kubernetes cluster.
* **API Gateway (Istio Ingress Gateway):** External API requests are routed through Istio Ingress Gateway.

Observability & CI/CD:

* **Monitoring (Prometheus & Grafana):** Application and infrastructure metrics are monitored using Prometheus and visualized with Grafana.
* **Distributed Tracing (Jaeger):** Request traces are collected and visualized using Jaeger for debugging and performance analysis.
* **CI/CD Pipeline (GitHub Actions):** Automated build, test, and deployment pipeline using GitHub Actions.
* **Blue/Green Deployments:** Implemented for seamless and zero-downtime deployments.

This project demonstrates best practices for building a production-ready cloud API, focusing on security, scalability, and observability.
