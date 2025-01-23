# Todo App 🚀

A simple RESTful API built with [Fiber](https://gofiber.io/) and MongoDB for managing a todo list.

---

## ✨ Features

- **Create** new todos with a body field and a completed status.
- **Read** all existing todos.
- **Update** the status of a todo (mark as completed).
- **Delete** a todo by ID.

---

## ✅ Prerequisites

Before you begin, ensure you have the following installed:

- [Go](https://go.dev/) (1.19 or later)
- [MongoDB](https://www.mongodb.com/)
- [Git](https://git-scm.com/)

---

## 🚀 Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/todo-app.git
   cd todo-app

2. Install dependencies:
    ```bash
    go mod tidy

3. Set up environment variables in a .env file in the root directory:
    ```bash
    MONGODB_URI=your-mongodb-connection-string
    PORT=5000

4. Run the app:
    ```bash
    go run main.go
    
---

## 🔗 API Endpoints
| Method | Endpoint         | Description              | Body Example                       |
|--------|------------------|--------------------------|-------------------------------------|
| GET    | `/api/todos`     | Retrieve all todos       | -                                   |
| POST   | `/api/todos`     | Create a new todo        | `{ "body": "Learn Go" }`           |
| PATCH  | `/api/todos/:id` | Update a todo as done    | -                                   |
| DELETE | `/api/todos/:id` | Delete a todo by ID      | -                                   |

```json
{
  "id": "64f25e2a1234567890abcdef",
  "completed": false,
  "body": "Finish writing the README"
}

