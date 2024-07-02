# Live Collaborative To-Do List

Welcome to the **Live Collaborative To-Do List**! This project allows multiple users to collaboratively manage a to-do list in real-time. Built using GUN, a decentralized database, this application ensures data synchronization across all connected users without the need for a centralized server.

## Demo

Check out the live demo here: [Live Collaborative To-Do List Demo](https://joe-shenouda.github.io/Live-Collaborative-To-Do-List/)

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [How It Works](#how-it-works)
- [Contributing](#contributing)
- [License](#license)
- [Acknowledgments](#acknowledgments)

## Introduction

The **Live Collaborative To-Do List** was developed to demonstrate the capabilities of real-time data synchronization using GUN. The primary goal of this project is to provide a simple yet effective way for users to manage tasks collaboratively, with changes reflecting instantly across all users.

## Features

- **Real-Time Synchronization**: Tasks added, updated, or removed are instantly synchronized across all connected users.
- **Decentralized Data Storage**: Uses GUN for decentralized storage, ensuring high availability and resilience.
- **User-Friendly Interface**: Simple and intuitive design for managing tasks.
- **Serverless**: No backend server required; everything runs on the client side.

## Technologies Used

- **GUN**: A decentralized database for real-time data synchronization.
- **HTML**: For the basic structure of the application.
- **CSS**: For styling the application.
- **JavaScript**: For application logic and interaction with GUN.

## Getting Started

Follow these steps to set up and run the project locally.

### Prerequisites

- A modern web browser (Chrome, Firefox, Safari, etc.)

### Installation

1. **Clone the repository:**

   ```bash
   git clone https://github.com/joe-shenouda/Live-Collaborative-To-Do-List.git
   cd Live-Collaborative-To-Do-List
   ```

2. **Open `index.html` in your web browser:**

   You can simply double-click on the `index.html` file or use a local server to serve the files.

   ```bash
   # For example, using Python's HTTP server:
   python -m http.server
   ```

   Navigate to `http://localhost:8000` in your browser.

## How It Works

### Real-Time Data Synchronization with GUN

The application connects to a GUN relay server hosted at `https://gun-manhattan.herokuapp.com/gun`. This setup ensures that tasks are instantly synchronized across all connected users.

### Adding a Task

When a user adds a new task, a unique ID is generated for the task, and it is added to the GUN database. The task is then rendered in the task list for all connected users.

### Removing a Task

When a user removes a task, it is deleted from the GUN database, and the task is removed from the task list for all connected users.

### Preventing Duplicate Tasks

To prevent duplicate tasks from being rendered, a `seenTasks` set is used to keep track of tasks that have already been rendered. Before rendering a task, the application checks if the task ID is in the `seenTasks` set.

## Contributing

Contributions are welcome! If you have any ideas, suggestions, or bug reports, feel free to open an issue or submit a pull request.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- **GUN**: For providing an excellent decentralized database solution.
- **Contributors**: To everyone who has contributed to the project.
- **Community**: For the support and feedback.

---

Thank you for checking out the **Live Collaborative To-Do List**! If you have any questions or feedback, feel free to reach out.

Joe Shenouda
