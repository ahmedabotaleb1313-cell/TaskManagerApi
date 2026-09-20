# Task Manager API

A RESTful API built with **ASP.NET Core** and **Entity Framework Core** for managing users and their tasks.

## 🚀 Features

- Full CRUD operations for Users
- Full CRUD operations for Tasks
- One-to-Many relationship between Users and Tasks
- SQL Server database integration via Entity Framework Core

## 🛠️ Tech Stack

- **Language:** C#
- **Framework:** ASP.NET Core Web API
- **ORM:** Entity Framework Core
- **Database:** SQL Server

## 📋 API Endpoints

### Users
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/users` | Get all users |
| GET | `/api/users/{id}` | Get a single user |
| POST | `/api/users` | Create a new user |
| DELETE | `/api/users/{id}` | Delete a user |

### Tasks
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/api/tasks` | Get all tasks |
| GET | `/api/tasks/{id}` | Get a single task |
| POST | `/api/tasks` | Create a new task |
| PUT | `/api/tasks/{id}` | Update a task |
| DELETE | `/api/tasks/{id}` | Delete a task |

## ⚙️ Getting Started

### Prerequisites
- .NET SDK
- SQL Server (Express or higher)

### Installation

1. Clone the repository
```bash
git clone https://github.com/ahmedabotaleb1313-cell/TaskManagerApi.git
```

2. Navigate to the project folder
```bash
cd TaskManagerApi
```

3. Update the connection string in `appsettings.json` if needed

4. Apply migrations to create the database
```bash
dotnet ef database update
```

5. Run the project
```bash
dotnet run
```

## 📦 Data Models

**User**
- Id, Username, Email, PasswordHash, Tasks (list)

**TaskItem**
- Id, Title, Description, IsCompleted, CreatedAt, UserId

## 📝 License

This project is open source and available for learning purposes.