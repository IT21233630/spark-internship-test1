Features
* Add a task
* Mark a task as completed
* Delete a task
* View the list of tasks
* In-memory storage (or H2 database for persistence)

Setup Instructions
1. Prerequisites
  Java 17+
  Maven 3+
  Postman (optional, for API testing)
2. How to Run the Application
  Extract the ZIP file into a folder.
  Open a terminal in the project root directory.
Run the following command to build and start the application:

mvn spring-boot:run

Once the application starts it will be available in
http://localhost:8080

3.  API Endpoints
   Method	Endpoint	    Description
   GET	    /tasks	    Get all tasks
   POST	    /tasks	    Add a new task
   PUT	    /tasks/{id}	Mark task as done
   DELETE	/tasks/{id}	Delete a task

4.  Using H2 Database
   Open your browser and go to:  
   http://localhost:8080/h2-console

   Use the following database details:
   JDBC URL: jdbc:h2:mem:testdb
   Username: sa
   Password: Abans
   Click Connect 
5.  Testing with Postman
    Import the API collection or manually send requests using the given endpoints.
    Example POST request body (JSON format):
    {
  "title": "Finish the project",
  "completed": false
}

