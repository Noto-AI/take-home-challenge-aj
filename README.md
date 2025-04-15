# Scheduling System Backend Service

This project is a backend service for managing a scheduling system inspired by **Noto**. It handles event scheduling on a calendar, specifically for educational sessions, such as group and private classes.

## 📚 Features

#### **Endpoint**
- Implement at least one core API endpoint to handle scheduling functionality (e.g., creating or retrieving scheduled sessions).
- You are encouraged to add additional endpoints if they improve the overall design or user experience.

### **Testing**
- Include test cases or test scripts to demonstrate that your backend service functions as expected.

## 🔌 Mock API Integration

#### **Endpoint**
`GET /staff-availability`

#### **Purpose**
Retrieve the availability of each staff member. Please implement a mock API with below response format.

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

1. create a bare clone of the repo: `git clone --bare git@github.com:Noto-AI/take-home-challenge-scheduler.git`.
2. Create a new private repository on Github for this take home challenge.
3. Mirror push your bare clone to your new git repo: `git push --mirror git@github.com:<your_username>/take-home-challenge-scheduler.git`.
4. Remove the temporary local repository you created in step 1 and clone your own take-home-challenge-1 repository on your machine.
5. when you finish your challenge, just open a pull request of your work, and add stevenwang223 as collaborator to view your PR. 

### Assumptions
In cases where the problem description is ambiguous or incomplete, feel free to make reasonable assumptions based on your judgment. Document any such assumptions in this section to clarify your design decisions and implementation approach.

## 📦 Deliverables

At a high level, your submission should include:

- A working backend service.

- Integration with the mock staff availability API.

- Clear documentation outlining setup, API usage, and assumptions made.

- A concise explanation of how your scheduling logic works.

- You are expected to make reasonable decisions about scope, edge cases, and any missing details.
