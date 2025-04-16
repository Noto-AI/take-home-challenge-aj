# Scheduling System Backend Service

This project is a backend service for managing a scheduling system inspired by **Noto**.

## Context

1. This app is for the owner/administrator of a tutoring center
2. This user is the central person who does the scheduling for all of our clients and instructors
3. This scheduling system will be for private lessons only: one instructor and one student

## Task + Requirements

Implement the backend service that fulfills the product requirements below

1. Create lessons, which would be one off or recurring (Tuesday's at 3PM)
2. Reschedule lessons, which might be for one lesson or for a batch (Tuesdays at 3PM -> Tuesdays at 4PM)
3. Delete lessons, which follows the same pattern as before

## 🔌 API's that you can assume exist

#### **Endpoint**
`GET /staff-availability`

#### **Purpose**
Retrieve the availability of each staff member. You can implement/mock an API with below response format.

#### **Response Format**
```json
[
  {
    "staff_id": "123",
    "staff_name": "Steve Wang",
    "start_date": "2025-01-10",
    "end_date": "2025-05-20",
    "blackout_dates": ["2025-02-12", "2025-03-15", "2025-04-12", "2025-05-15"]
  }
]
```

- `start_date`: Beginning of available period
- `end_date`: End of available period
- `blackout_dates`: List of dates when the staff member is unavailable (e.g., holidays, vacations)

## 🛠 Tech Stack

- **Node.js**
- **PostgreSQL**
- **Drizzle ORM**

## 🧪 Documentation & Testing

### Setup Instructions

	1.	Push your implementation to your GitHub repo alone along with a copy of this README
	2.	Open a pull request with a brief summary of your work and any assumptions.
	3.	Add stevenwang223 as a collaborator so we can access and review your PR.

### Assumptions
In cases where the problem description is ambiguous or incomplete, feel free to make reasonable assumptions based on your judgment. Document any such assumptions in this section to clarify your design decisions and implementation approach.

## 📦 Deliverables

At a high level, your submission should include:

- A working backend service.

- Integration with the mock staff availability API.

- Clear documentation outlining setup, API usage, and assumptions made. 

- A concise explanation of how your scheduling logic works.

- You are expected to make reasonable decisions about scope, edge cases, and any missing details.

- Include test cases or test scripts to demonstrate that your backend service functions as expected.

## Expectations
- You are encouraged to use whichever AI tool you prefer to help with the task.
- You are not expected to spend more than 2-4 hours on the takehome.
- The project is intentinoally very open-ended, so prioritize whatever you can within the time constraints.

## Bonus points

- a frontend app

