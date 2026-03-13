# school_api
A robust Node.js and Express-based API designed to manage school data. This project allows users to add new schools and retrieve a list of existing schools sorted by their geographical proximity to a user-provided location.

## Live Demo
- **API URL:** https://school-api-e6n3.onrender.com
- **Database:** MySQL (Hosted on Aiven.io)

## Features
- **Add School:** `POST /addSchool` - Validates and stores school information (name, address, latitude, and longitude).
- **List Schools:** `GET /listSchools` - Retrieves all schools from the database and uses the **Haversine Formula** to sort them based on distance from the user's coordinates.

## Tech Stack
- **Backend:** Node.js, Express.js
- **Database:** MySQL (Aiven Cloud)
- **Deployment:** Render.com
- **Tools:** Postman, Git

## Database Schema
The database consists of a `schools` table with the following structure:
- `id`: Primary Key (Auto-increment)
- `name`: String (Required)
- `address`: String (Required)
- `latitude`: Float (Required)
- `longitude`: Float (Required)

## Getting Started

### Prerequisites
- Node.js installed locally
- Aiven MySQL connection details
- `ca.pem` SSL certificate (required for Aiven connections)

### Installation
1. Clone the repository:
   ```bash
   git clone [https://github.com/Purvashi04/school_api.git](https://github.com/Purvashi04/school_api.git)
   cd school_api
