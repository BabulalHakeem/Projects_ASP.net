Project Title: ToDo List REST API

Description:
This project is a simple REST API for managing a ToDo list. It allows users to create, read, update, and delete tasks. The project is built using ASP.NET Core, and data is stored in an in-memory database for simplicity.

Features:
Create a new task
View all tasks
Update a task
Delete a task


Prerequisites:
Install .NET 6 SDK or later.
Install a code editor like Visual Studio or Visual Studio Code.
Basic understanding of REST APIs and tools like Postman or any browser-based API testing tool.

Steps to Run the Project:
1. Clone the Repository
Open a terminal or command prompt.

Run the following command to clone the repository:

git clone https://github.com/your-username/todo-list-api.git

Navigate to the project folder:

cd todo-list-api

3. Restore Dependencies
   
Open the project in Visual Studio or navigate to the project folder in the terminal.
Restore NuGet packages by running:
dotnet restore

5. Build the Project
In the terminal, run the following command to build the project:
dotnet build
Ensure there are no build errors before proceeding.

6. Run the Project
Use the command below to start the API:
dotnet run
The API will start running, and you will see the base URL (e.g., https://localhost:5001).

8. Test the API
Use Postman or any REST client to interact with the API. Below are the endpoints:

Method	Endpoint	Description
GET	/api/todos	Get all tasks
GET	/api/todos/{id}	Get a task by ID
POST	/api/todos	Create a new task
PUT	/api/todos/{id}	Update a task by ID
DELETE	/api/todos/{id}	Delete a task by ID
Example:
To create a new task:
Use the POST method with the URL https://localhost:5001/api/todos.
In the body, send:

{
  "title": "Sample Task",
  "description": "Complete the README file"
}
To view all tasks:
Use the GET method with the URL https://localhost:5001/api/todos.

6. Stopping the Server
Press Ctrl+C in the terminal to stop the server.

Directory Structure:

|-- ToDoListApi/
    |-- Controllers/
    |   |-- TodoController.cs  # Handles API endpoints
    |-- Models/
    |   |-- Todo.cs            # Task data structure
    |-- Program.cs             # Entry point of the application
    |-- appsettings.json       # Configuration file
Known Issues:
This project uses an in-memory database. All data will reset when the application is stopped.
No authentication/authorization has been implemented.

Future Enhancements:
Add persistent database support (e.g., SQL Server, MongoDB).
Implement authentication and user management.

Author: Babulal H
Email: babulalhakeem@gmail.com
