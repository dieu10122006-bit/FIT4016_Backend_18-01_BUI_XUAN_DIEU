# School Management API

## Project Information
- **Course**: FIT4016 – Backend Programming
- **Student**: (Your name here)
- **Year**: 2026
- **Technology**: ASP.NET Core Web API, Entity Framework Core
- **Database**: SQL Server
- **IDE**: Visual Studio Code

---

## Description
This project is a backend application for managing **Schools** and **Students** using **Entity Framework Core**.

The system supports:
- One-to-many relationship between Schools and Students
- CRUD operations for Students
- Input validation
- Pagination
- User-friendly error messages in English

---

## Database Structure

### Table: Schools
- Id (int, primary key, auto increment)
- Name (string, unique, not null)
- Principal (string, not null)
- Address (string, not null)
- CreatedAt (datetime)
- UpdatedAt (datetime)

### Table: Students
- Id (int, primary key, auto increment)
- SchoolId (foreign key)
- FullName (string, not null)
- StudentId (string, unique, not null)
- Email (string, unique, not null)
- Phone (string, nullable)
- CreatedAt (datetime)
- UpdatedAt (datetime)

---

## Technologies Used
- ASP.NET Core Web API
- Entity Framework Core (Code First)
- SQL Server
- REST Client (.http file)
- Git for version control

---

## How to Run the Project

1. Open the project in Visual Studio Code
2. Restore packages:
   ```bash
   dotnet restore
