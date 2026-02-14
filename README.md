# 🍔 FoodStore — Microservices Food Ordering System  
**(Advanced Programming Course Project)**

## 📌 About the Project

**FoodStore** is a university **Advanced Programming course project** that demonstrates a microservices-based food ordering system built with **Go (Golang)**.

The project focuses on practical backend engineering topics such as:
- Microservices architecture  
- API Gateway pattern  
- Inter-service communication with **gRPC**  
- Layered architecture and clean code practices  
- Basic testing and modular design  

The system consists of multiple independent services and a simple frontend client.

---

## 🏗️ Architecture

The project is structured as a set of microservices:

- **API Gateway** — entry point for clients, routes requests to backend services  
- **Menu Service** — manages food items and menu  
- **Order Service** — handles orders and order processing logic  
- **User Service** — manages users  
- **Payment Service** — handles payment logic  
- **Frontend** — simple client interface  

Each service follows a layered structure:
- `handler` — HTTP/gRPC handlers  
- `service` — business logic  
- `dao` / `repository` — data access layer  
- `model` — domain models  

Services communicate with each other using **gRPC**.

---

## 🛠️ Tech Stack

- **Language:** Go (Golang)  
- **Architecture:** Microservices, Layered Architecture  
- **Communication:** gRPC  
- **API:** REST (via API Gateway)  
- **Tools:** Git, Go Modules  
- **Testing:** Go testing (basic unit tests)  

---

## ✨ Features

- Microservices-based backend architecture  
- API Gateway for request routing  
- CRUD operations for:
  - Users  
  - Menu items  
  - Orders  
- gRPC-based communication between services  
- Clean separation of concerns using layered design  
- Basic business logic and validations  

---

## 📂 Project Structure (Simplified)

```bash
FoodStore/
├── APIGATEWAY/
├── Menu_service/
├── Order_service/
├── User_service/
├── Payment_service/
├── Frontend/
└── README.md

## 📦 Service Structure

Each service contains:

```bash
├── handler/
├── service/
├── dao/ (or repository/)
├── model/
└── main.go

---

## 🚀 How to Run (Example)
⚠️ Note: Each service should be run separately.

Clone the repository:
git clone https://github.com/your-username/FoodStore.git
cd FoodStore
Run a service (example: Menu Service):
cd Menu_service
go run main.go
Run API Gateway:
cd APIGATEWAY
go run main.go
Start other services in the same way and use the system via the API Gateway or frontend.

---

## 🎓 Educational Purpose

This project was created as part of a university Advanced Programming course to practice:
Designing and implementing microservices
Building an API Gateway
Using gRPC for inter-service communication
Structuring backend applications with layered architecture
Writing clean, modular, and maintainable Go code

---

## 👨‍💻 Author
Olzhas Karabekov
Advanced Programming Course Project

---

## 📄 License
This project is for educational purposes only.
