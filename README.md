### **Obywatel Plus Infrastructure & Monorepo**

This repository hosts the **Obywatel Plus** ecosystem, a high-performance microservices platform built with **Go** and **Fiber**. The project utilizes a shared **Platform Core** to ensure consistency in security, observability, and data management across all services.

#### **Core Infrastructure Components**
*   **Edge Layer:** **Ingress Nginx** (Work in Progress) – Configured to handle centralized routing, SSL termination, and traffic orchestration.
*   **Shared Platform (`/pkg`):** A unified internal framework providing standardized drivers for **PostgreSQL**, **Redis** (with Lua rate-limiting), and **OpenTelemetry**.
*   **Service Mesh:** 5 specialized microservices (Auth, Citizen-Docs, Gateway, Notifications, Audit) orchestrated via **Docker Compose** and **Go Workspaces**.
*   **Security:** Multi-layered protection using **Docker Secrets**, HMAC validation, and centralized JWT management.

WIP