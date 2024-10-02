# Task Tracker

A simple web application to help users manage their tasks efficiently. Users can create, edit, and delete tasks, set deadlines, and track their progress.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Contact](#contact)

## Features

- **User Authentication**: Secure login and registration.
- **Task Management**: Create, edit, and delete tasks with due dates.
- **Progress Tracking**: Mark tasks as completed.
- **Filter & Sort**: Organize tasks by deadline, status, or priority.
- **Responsive Design**: Mobile-friendly interface.

## Installation

To set up the project locally, follow these steps:

1. Clone the repository:
    ```bash
    git clone https://github.com/yourusername/task-tracker.git
    cd task-tracker
    ```

2. Install the necessary dependencies:
    ```bash
    npm install
    ```

3. Set up environment variables. Create a `.env` file in the root directory with the following:
    ```plaintext
    DATABASE_URL=your_database_url
    JWT_SECRET=your_jwt_secret
    ```

4. Start the development server:
    ```bash
    npm run dev
    ```

## Usage

After the server is running, you can access the application at `http://localhost:3000`.

### Creating a Task

1. Log in to your account.
2. Click on the "Add Task" button.
3. Fill in the task details and set a due date.
4. Click "Save" to add the task to your list.

### Example API Call

To create a new task via the API, you can use the following `curl` command:

```bash
curl -X POST http://localhost:3000/api/tasks \
-H "Content-Type: application/json" \
-d '{"title": "Finish project report", "dueDate": "2024-10-15"}'
