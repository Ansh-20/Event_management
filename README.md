# Event Management Dashboard

## Objective
To develop a complete Event Management Dashboard featuring a React.js frontend, a Django backend for the admin panel, and an Express.js microservice for additional API functionalities.

---

## Project Overview

The Event Management Dashboard is a full-stack application designed to manage events efficiently. It includes features for listing, adding, editing, and analyzing events, with robust authentication and a modern, user-friendly interface.

---

## Features

### Frontend (React.js)
- **Responsive and User-Friendly Interface**
- **Pages and Components**:
  - **Event List Page**: Displays all events with search and filter options.
  - **Event Detail Page**: Shows details of a selected event.
  - **Add/Edit Event Page**: Includes a form to add or edit an event.
- **Navigation**: Implemented using React Router.
- **State Management**: Handled using Redux Toolkit or React Context API.
- **Calendar Integration**: Integrated a calendar UI (e.g., FullCalendar).
- **Form Validations**: Ensures proper data entry for events.
- **API Integration**: Fetches data using Axios or Fetch API.
- **Error Handling**: Displays error messages for failed API calls.

### Backend (Express, Node)
- **Admin Panel**: Provides CRUD operations for event management.
- **API Endpoints** (using Django REST Framework):
  - `GET /api/events/` - Fetch all events.
  - `POST /api/events/` - Add a new event.
  - `PUT /api/events/<id>/` - Update an event.
  - `DELETE /api/events/<id>/` - Delete an event.
- **Models**:
  - `Event`: Includes fields like `title`, `description`, `start_date`, `end_date`, `location`, `created_at`, and `updated_at`.
- **Authentication**: Secures API endpoints with token-based authentication.

### Microservice (Express.js)
- **Analytics API**:
  - `GET /analytics/event-count` - Returns the total number of events.
  - `GET /analytics/upcoming-events` - Returns a list of upcoming events.
- **Logging Service**:
  - Logs API usage and event-related changes into MongoDB using Mongoose.
- **Authentication**: Secures endpoints with JWT-based authentication.

### Integration
- **Frontend-Backend Integration**:
  - Connects React frontend with Django and Express.js backends.
  - Utilizes environment variables for API URLs.
- **Authentication Flow**:
  - Implements login/logout system using JWT tokens.
  - Secures React routes based on authentication.

### Testing
- **Express.js**: Unit tests for routes using Mocha or Jest.
- **React**: Tests components and API integration using Jest and React Testing Library.
---

## Setup Instructions

### Prerequisites
- **Node.js** (v16+)
- **MongoDB**
- **React.js**
- **Express**



#### Microservice (Express.js)
1. Navigate to the microservice directory.
   ```bash
   cd microservice
   ```
2. Install dependencies.
   ```bash
   npm install
   ```
3. Start the Express server.
   ```bash
   npm start
   ```

#### Frontend (React.js)
1. Navigate to the frontend directory.
   ```bash
   cd frontend
   ```
2. Install dependencies.
   ```bash
   npm install
   ```
3. Start the React application.
   ```bash
   npm start
   ```

---



## Author
Developed by Ansh Soni.


