# Report Generator

## Overview
The Report Generator is a Java-based Maven project designed to manage and generate reports for student records. It utilizes JDBC for MySQL as the backend database and demonstrates the use of Object-Oriented Programming (OOP) concepts such as polymorphism (function overloading) and data abstraction. The project also leverages the iText library to create PDFs of student reports, detailing their marks and other information. The entire GUI is implemented using Swing JFrame, providing a single-window interface for all operations.

## Features
- **Add Student Records**: Allows adding new student records through the GUI.
- **Update Student Records**: Provides functionality to update existing student records.
- **Delete Student Records**: Enables deletion of student records from the database.
- **View and Download Reports**: Generates a PDF report of student marks and details, which can be downloaded.
- **Database Operations**: Utilizes SQL joins, primary keys, and foreign keys for efficient database management.

## Technologies Used
- **Java**
- **Maven**
- **JDBC (Java Database Connectivity)**
- **MySQL**
- **iText PDF**
- **Swing (JFrame)**

## OOP Concepts
- **Polymorphism (Function Overloading)**
- **Data Abstraction**

## Installation and Setup
1. **Clone the Repository**:
    ```bash
    git clone https://github.com/Javed0-786/Report-Generator
    cd report-generator
    ```

2. **Setup Database**:
    - Create a MySQL database.
    - Import the provided SQL script to set up the tables and relationships.

3. **Configure Database Connection**:
    - Update the database configuration in the project to match your MySQL database settings.

4. **Build the Project**:
    ```bash
    mvn clean install
    ```

5. **Run the Application**:
    ```bash
    java -jar target/report_generator-1.0-SNAPSHOT.jar
    ```

## Usage
- **Login Window**: Start the application and login using your credentials.
- **Add Student**: Navigate to the 'Add Student' section to add new student records.
- **Update/Delete Student**: Use the 'Manage Students' section to update or delete existing records.
- **View Marks**: Navigate to the 'View Marks' section to view student marks and download PDF reports.

## GUI Components
- **Main Login Window**: The initial window for user login.
- **Single Window Interface**: All functionalities (add, update, delete, view) are accessible through a single window interface.

## Example Code Snippets
### Main.java
```java
package com.example;

public class Main {
    public static void main(String[] args) {
        MainLoginWindow login = new MainLoginWindow();
        login.setVisible(true);
    }
}
