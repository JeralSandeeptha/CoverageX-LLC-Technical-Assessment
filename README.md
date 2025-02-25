# To-Do Task Web Application

This repository contains all the project details for a CoverageX LLC technical assignment The project is designed to run seamlessly, providing a high quality frontend and backend repositories for demonstration purposes.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [Database](#database)
- [Source Code Management](#source-code-management)
- [Main Focus](#main-focus)
- [Extra Considerations](#extra-considerations)
- [Source Code](#source-code)
- [Improvements](#improvements)
- [Future Enhancements](#future-enhancements)
- [Acknowledgment](#acknowledgment)

## Overview

This project is a full-stack to-do task web application built using a monolithic architecture. The application allows users to create, view, and manage tasks efficiently. It adheres to clean code principles and SOLID design patterns to ensure maintainability and scalability.

## Features

Users can create tasks with a title and description

Only the five most recent tasks are displayed

Users can mark tasks as "Done," which removes them from the UI

The system follows a monolithic architecture

All components are containerized using Docker and managed with docker-compose

Unit, Intergration and End to End testing should be done through relavant areas

## Technologies Used

Frontend: React (TypeScript, Vite)

Backend: Express.js with TypeScript

Database: PostgreSQL

Testing:
- Unit Testing: Vitest
- End-to-End Testing: Cypress

Containerization: Docker & Docker Compose

API Testing - Postman

API Documentation - Thorugh Postman Publisher

UI Libraries - Material UI

## System Architecture

## Database

## Source Code Management

## Main Focus

## Extra Considerations

Implement user authentication for task management

Advance user management with access Tokens and refresh tokens

## Source Code

## Improvements

1. Enhancing Performance and Scalability
 - Implement server-side pagination for task retrieval instead of limiting the UI to 5 tasks
 - Optimize database queries with indexing for faster retrieval
 - Use caching mechanisms like Redis to store frequently accessed data.

2. Code Quality and Best Practices
 - Enhance error handling with proper status codes and meaningful messages.

3. Security Enhancements
 - Improve the security with two factor authentication.

4. Database and API Improvements
 - Implement API versioning to maintain backward compatibility.

5. Improved Testing Strategy
 - Improve the test coverage of the code base.

6. Docker and Deployment Enhancements
 - Optimize Docker image sizes by using multi-stage builds.
 - Implement a CI/CD pipeline for automated testing and deployment.

## Future Enhancements

Implement user authentication for task management

Introduce real-time task updates using WebSockets

Enhance UI/UX with better animations and state management

Optimize database queries with indexing for better performance

Implement server-side pagination to handle large datasets

Add role-based access control (RBAC) for different user levels

Deploy the application to a cloud platform with CI/CD integration

## Acknowledgment

Thank you for taking the time to review this project. Your feedback is greatly appreciated. Thanks for the CoverageX LLC company to reviewing this technical assignment. For those who refer this project, if you find this project useful, feel free to star the repository on GitHub and share it with others! 