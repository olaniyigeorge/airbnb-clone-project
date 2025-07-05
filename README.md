# Airbnb Clone Project

## Overview

The **Airbnb Clone Project** is a comprehensive backend-focused web application inspired by Airbnb. It aims to simulate building a robust, scalable, and secure booking platform. This project provides hands-on experience with modern backend development using **FastAPI**, **PostgreSQL**, and **RESTful APIs**, while also emphasizing collaboration, CI/CD workflows, and database architecture.

## Project Goals

- Design and build a backend system for a booking platform.
- Implement secure and well-documented RESTful APIs.
- Model and manage a relational database using PostgreSQL.
- Apply CI/CD principles using GitHub Actions and Docker.
- Collaborate using Git and GitHub effectively.

---

## Technology Stack

- **Backend Framework**: FastAPI
- **Database**: PostgreSQL
- **API Style**: REST
- **Containerization**: Docker
- **CI/CD**: GitHub Actions
- **Version Control**: Git + GitHub
- **Testing**: Pytest

---

## Team Roles

### 1. Backend Developer
Implements core application logic, RESTful APIs, authentication, authorization, and business rules using FastAPI. Ensures code quality and maintainability.

### 2. Database Administrator (DBA)
Designs and maintains the PostgreSQL database schema. Defines tables, relationships, constraints, indexes, and handles migrations and performance tuning.

### 3. DevOps Engineer
Responsible for Docker setup, GitHub Actions pipelines, environment configuration, and deployment automation to ensure consistent integration and delivery.

### 4. Security Specialist
Handles authentication systems (e.g., JWT), role-based access control, rate limiting, and protects APIs against vulnerabilities like SQL injection, XSS, and CSRF.

### 5. Documentation Lead
Manages project documentation including the README, API reference, setup guides, and database schema diagrams. Ensures clarity and ease of use for contributors.

---

## Database Design

The application uses a normalized relational schema in PostgreSQL with the following key entities:

- **Users** – stores user account data (name, email, password hash, etc.)
- **Properties** – includes listing data such as name, description, location, price, etc.
- **Bookings** – tracks reservations made by users for properties.
- **Payments** – stores payment status and transaction info tied to bookings.

All relationships are properly defined with foreign keys and indexes to ensure fast query performance.

---

## Feature Breakdown

The core features of the Airbnb Clone include:

- **User Registration & Login**: JWT-based authentication.
- **Property Listings**: Users can view and list properties.
- **Booking System**: Bookings are tied to properties and users, with date validation.
- **Payment Tracking**: Simulated payment processing tied to bookings.
- **Role Management**: Admins and regular users have different access levels.
- **API Documentation**: Swagger/OpenAPI auto-generated from FastAPI.

---

## API Security

Security measures implemented in this project:

- **JWT Authentication**: Secure token-based login system.
- **Password Hashing**: All passwords stored using industry-standard hashing (e.g., bcrypt).
- **Role-Based Access Control**: Only authorized users can access specific endpoints.
- **Input Validation**: Pydantic models used to validate request data.
- **CORS Configuration**: Controlled cross-origin access.
- **Rate Limiting** *(optional extension)*: Protects endpoints from abuse.

---

## CI/CD Pipeline

The project uses GitHub Actions to automate the development workflow:

- **Linting & Testing**: Code is linted and tested automatically on every push.
- **Docker Build**: Application is built inside a Docker container for consistent environments.
- **Deployment Steps**: Future integration planned for staging and production deployments.

Example Workflow File: `.github/workflows/main.yml`

---

## Repository

- **GitHub Repository**: [airbnb-clone-project](https://github.com/olaniyigeorge/airbnb-clone-project.git)

---

## Getting Started

1. **Clone the Repository**
   ```bash
   git clone https://github.com/olaniyigeorge/airbnb-clone-project.git
   cd airbnb-clone-project
