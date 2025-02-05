# Online Learning System - Django Based

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Project](#running-the-project)
- [API Documentation](#api-documentation)
- [Caching](#caching)
- [Real-Time Features](#real-time-features)
- [Development Roadmap](#development-roadmap)
- [Contributing](#contributing)
- [License](#license)

## Introduction
The Online Learning System is a robust, feature-rich platform built using Django. It provides a comprehensive environment for instructors to manage courses and students to enroll and interact with diverse educational content. The system incorporates essential content management features, authentication mechanisms, real-time updates, and API endpoints for integration.

## Features

### Core CMS Functionality
- Create and manage course models.
- Support for polymorphic content using model inheritance.
- Custom model fields for flexible data handling.
- Ordering capabilities for course contents and modules.
- Authentication views for the CMS.

### Content Management
- Class-based views and mixins for CMS operations.
- Formsets and model formsets for editing course modules and contents.
- Drag-and-drop functionality for reordering modules and contents.
- Group and permission management for access control.

### Student and Public Views
- Public views for course information display.
- Student registration and course enrollment.
- Diverse content rendering for course modules.

### Caching
- Installation and configuration of Memcached.
- Content caching using Django’s cache framework.
- Support for Memcached and Redis backends.
- Redis server monitoring in Django Admin.

### RESTful API Development
- Installation and configuration of Django REST Framework (DRF).
- Serializers and nested serializers for model data.
- Custom API views and API authentication.
- Permissions and custom permission classes.
- Implementation of ViewSets and routers.
- API consumption using the Requests library.

### Real-Time Features
- ASGI support for asynchronous operations.
- WebSocket integration with Django Channels.
- Fully asynchronous WebSocket consumer.
- Real-time communication using Redis channel layers.
- WebSocket client implementation.

## Installation

### Prerequisites
- Python 3.x
- PostgreSQL
- Redis
- Docker & Docker Compose
- Node.js (for WebSocket client integration)

### Steps
1. Clone the repository:
   ```bash
   git clone <repository-url>
   cd <project-directory>
   ```
2. Create a virtual environment:
   ```bash
   python3 -m venv venv
   source venv/bin/activate
   ```
3. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
4. Apply migrations:
   ```bash
   python manage.py migrate
   ```
5. Load initial data (fixtures):
   ```bash
   python manage.py loaddata <fixture-file>
   ```
6. Run the development server:
   ```bash
   python manage.py runserver
   ```

## Configuration
- Rename `.env.example` to `.env` and update environment variables.
- Set up Redis and PostgreSQL configurations in `settings.py`.
- Configure caching backend options.

## Running the Project
To start the application:
```bash
python manage.py runserver
```

To use Docker Compose:
```bash
docker-compose up --build
```

## Contributing
Contributions are welcome! Please follow these steps:
1. Fork the repository.
2. Create a feature branch: `git checkout -b feature-name`
3. Commit your changes: `git commit -m "Add feature"`
4. Push to the branch: `git push origin feature-name`
5. Open a pull request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.

