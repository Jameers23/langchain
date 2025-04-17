# Project Overview

This project is a FastAPI application that provides a RESTful API for managing leaves and pods.

## Endpoints

### GET /api/dashboard/tiles
Returns dashboard tiles.

### POST /api/lms/leaves/apply
Applies for a leave.

### PATCH /api/lms/leaves/{leave_id}/approve
Approves a leave.

### GET /api/pods/{pod_id}/details
Returns pod details.

### POST /api/pods/{pod_id}/recommend
Recommends a pod.

### POST /api/auth/login
Logs in a user.

### GET /api/auth/user
Returns the current user.

## Project Structure

The project is structured as follows:

- app/
  - api/
    - routes/
      - dashboard_tiles.py
      - lms_leaves_apply.py
      - lms_leaves_approve.py
      - pods_details.py
      - pods_recommend.py
      - auth_login.py
      - auth_user.py
    - services/
      - database.py
    - main.py
  - models/
    - leaves.py
    - pods.py
    - users.py

## How to Run

To run the project, navigate to the root directory and execute the following command:

```bash
uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```