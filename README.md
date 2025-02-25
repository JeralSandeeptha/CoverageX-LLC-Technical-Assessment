# To-Do Task Web Application

This repository contains all the project details for a CoverageX LLC technical assignment The project is designed to run seamlessly, providing a high quality frontend and backend repositories for demonstration purposes.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [System Architecture](#system-architecture)
- [Database Architecture](#database-architecture)
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

Follow user stories documentation for more details. [View User Stories Documentation](https://docs.google.com/document/d/1fKk21F5OHyZoVNSG5bwFx0rX9dtmRW2ckO6F6w_Pbno/edit?tab=t.0)

- Users can create tasks with a title and description
- Only the five most recent tasks are displayed
- Users can mark tasks as "Done" which removes them from the UI
- The system follows a monolithic architecture
- All components are containerized using Docker and managed with docker-compose
- Unit, Intergration and End to End testing should be done through relavant areas

## Technologies Used

- Frontend: React (TypeScript, Vite)
- Backend: Express.js with TypeScript
- Database: PostgreSQL
- Testing: Unit Testing: Vitest, End-to-End Testing: Cypress
- Containerization: Docker & Docker Compose
- API Testing - Postman
- API Documentation - Thorugh Postman Publisher
- UI Libraries - Material UI
- Code Editor - Visual Studio Code

## System Architecture

This project was developed through Monolithic Architecture approach.

![System Architecture](src/architecture.png)

## Database Architecture

Run this query for create the database.
```sql
CREATE TABLE IF NOT EXISTS users (
    id SERIAL PRIMARY KEY,
    email VARCHAR(100) UNIQUE NOT NULL,
    password VARCHAR(255) NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

CREATE TABLE IF NOT EXISTS task (
    id SERIAL PRIMARY KEY,
    title VARCHAR(100) NOT NULL,
    description VARCHAR(255) NOT NULL,
    userId VARCHAR(255) NOT NULL,
    isCompleted BOOLEAN NOT NULL,
    created_at TIMESTAMP DEFAULT CURRENT_TIMESTAMP
);

SELECT * FROM task;
SELECT * FROM users;
```

## Main Focus

- Implement Task management
- Maintain code quality with testing
- Project should run on docker

## Extra Considerations

- Implement user authentication for task management
- Advance user management with access Tokens and refresh tokens

## Source Code Management

**Version Control**: Git with GitHub for source code management.

**Branching Strategy**: 
- main branch: Stable production-ready code.
- dev branch: Active development branch.
- test branch: Used for testing new features before merging to dev.
- hotfix branch: Used for critical bug fixes and emergency patches.

## Source Code

You can view the source code with following links.
- [Go to Frontend Repository](https://github.com/JeralSandeeptha/CoverageX-LLC-Technical-Assessment-React)
- [Go to Backend Repository](https://github.com/JeralSandeeptha/CoverageX-LLC-Technical-Assessment-Nodejs)

## Improvements

1. **Enhancing Performance and Scalability**
 - Implement server-side pagination for task retrieval instead of limiting the UI to 5 tasks
 - Optimize database queries with indexing for faster retrieval
 - Use caching mechanisms like Redis to store frequently accessed data.

2. **Code Quality and Best Practices**
 - Enhance error handling with proper status codes and meaningful messages.

3. **Security Enhancements**
 - Improve the security with two factor authentication.

4. **Database and API Improvements**
 - Implement API versioning to maintain backward compatibility.

5. **Improved Testing Strategy**
 - Improve the test coverage of the code base.

6. **Docker and Deployment Enhancements**
 - Optimize Docker image sizes by using multi-stage builds.
 - Implement a CI/CD pipeline for automated testing and deployment.

## Future Enhancements

- Implement user authentication for task management
- Introduce real-time task updates using WebSockets
- Enhance UI/UX with better animations and state management
- Optimize database queries with indexing for better performance
- Implement server-side pagination to handle large datasets
- Add role-based access control (RBAC) for different user levels
- Deploy the application to a cloud platform with CI/CD integration

## Acknowledgment

Thank you for taking the time to review this project. Your feedback is greatly appreciated. Thanks for the CoverageX LLC company to reviewing this technical assignment. For those who refer this project, if you find this project useful, feel free to star the repository on GitHub and share it with others! 