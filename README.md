# Sawing Profiles Management Application

## Description

A Python-based application designed to manage sawing profiles for industrial saw machines. This system features two main user roles:

- **Admin**: Responsible for creating and modifying sawing profiles, managing customer information, and overseeing the system configuration.
- **Operator**: Focused on selecting and executing profiles on the machine, as well as monitoring running operations.

The application simulates the execution of sawing profiles, including run-time statistics and performance data. All relevant information is stored in a database for later retrieval and analysis.

## Features

### Authentication

- [ ] Login system
- [ ] User credentials management
- [ ] Sign up functionality
- [ ] Role-based access (Admin vs. Operator)

### Admin Features

- [ ] Profile Management
  - [ ] Create, edit, and view sawing profiles
  - [ ] Manage advanced profile parameters (speed, force, material type)
  - [ ] Batch processing support
- [ ] Customer & Machine Management
  - [ ] Maintain a list of customer machines
  - [ ] Track which profiles are loaded on each machine
  - [ ] Record which user performed the upload
- [ ] Machine Integration
  - [ ] Upload profiles to the machine
  - [ ] Start/Stop profile execution
  - [ ] Collect run-time data for each machine

### Operator Features

- [ ] Profile Operations
  - [ ] View and select available sawing profiles
  - [ ] Upload selected profile to the machine
  - [ ] Start/Stop the sawing operation
- [ ] Machine Monitoring
  - [ ] View real-time status
  - [ ] Access logged run-time statistics

### Profile Parameters

- [ ] Technical Specifications
  - [ ] Cutting speed
  - [ ] Cutting force
  - [ ] Material type
  - [ ] Batch processing settings

### Statistics & Visualization

- [ ] Weekly or monthly run-time summaries
- [ ] Graphical displays of machine usage
- [ ] Historical data logging

## Technologies

- **Backend**: Python (Django)
- **Database**: PostgreSQ
- **Frontend**: HTML/CSS/JS + Bootstrap + Chart.js

## Goals

1. Provide a clear separation of roles (Admin vs. Operator), each with distinct capabilities.
2. Enable comprehensive profile management, including batch processing settings.
3. Offer machine-level tracking for loaded profiles and user interactions.
4. Gather and display run-time statistics, facilitating real-time and historical monitoring.
5. Ensure the application is testable, maintainable, and version-controlled using Git & GitHub.

## Git Workflow & Conventions

1. **Branching**
   - Create a new branch for each feature or bug fix.
   - **Naming Convention**: Use short prefixes indicating the purpose of the branch, for example:
     - `feat/<short-description>` for new features
     - `fix/<short-description>` for bug fixes
     - `docs/<short-description>` for documentation changes
     - `test/<short-description>` for test-related improvements
     - `refactor/<short-description>` for code refactoring

## Setup & Usage

1. **Install Dependencies**: Use a `requirements.txt` file for Python libraries.
2. **Run Backend**: Start the Django development server by running the following commands:

```bash
python manage.py migrate  # Apply database migrations
python manage.py runserver  # Start the Django server
```

3. **Run Frontend**: Open HTML page in your browser
4. **Login & Test**: Create an admin account, add new profiles, and run simulations as the operator.
