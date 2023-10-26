# Trove High-Level System Design

## Overview

Trove is a mobile application utilizing a client-server architecture. The client is built using the Flutter framework, following the MVVM architecture pattern with the Stacked library. The server, implemented in Node.js using TypeScript, employs the Express framework. Data is stored in a PostgreSQL database, managed through the Prisma ORM.

## Client (Flutter)

### Technologies and Architecture

- **Framework:** Flutter
- **Architecture:** MVVM using Stacked
- **Folder Structure:**

```plaintext
lib/
|-- models/
|-- view/
|-- viewmodels/
|-- services/
|-- utils/
|-- main.dart
```

### Naming and Code Organization Rules

- **File Naming:** Use descriptive names. For example, `user_profile_view.dart`.
- **Class Naming:** Follow PascalCase for class names. For example, `UserProfileView`.
- **Function Naming:** Use camelCase for function names. For example, `getUserProfileData`.
- **Variable Naming:** Follow camelCase for variable names. For example, `searchQuery`.
- **Code Organization:** Group related functionalities together. Utilize separate folders for models, views, viewmodels, services, and utility functions.

### Features

- **Search Bar with Autocomplete:**
  - Allow users to search for items with a responsive autocomplete feature, enhancing the user experience.

## Server (Node.js with TypeScript)

### Technologies and Architecture

- **Server Side Language:** Node.js with TypeScript
- **Framework:** Express
- **Folder Structure:**

```plaintext

src/
|-- controllers/
|-- routes/
|-- services/
|-- repositories/
|-- exeptions/
|-- utils/
app.ts
```

### Naming and Code Organization Rules

- **File Naming:** Use descriptive names. For example, `userController.ts`.
- **Class Naming:** Follow PascalCase for class names. For example, `UserController`.
- **Function Naming:** Use camelCase for function names. For example, `getUserData`.
- **Variable Naming:** Follow camelCase for variable names. For example, `userData`.
- **Code Organization:** Organize code into separate folders for controllers, routes, services, and models for a clear separation of concerns.

### Features

- **Define API Endpoints:**
  - Implement RESTful API endpoints to handle client requests, ensuring a smooth flow of data between the client and server.

## Database (PostgreSQL)

### Technologies and Architecture

- **Database:** PostgreSQL
- **ORM:** Prisma

### Naming and Code Organization Rules

- **Table Naming:** Use snake_case for table names. For example, `user_profiles`.
- **Column Naming:** Use snake_case for column names. For example, `first_name`.
- **Code Organization:** Define database schemas, models, and queries in separate files for a clean and organized database layer.
  
## Additional Development Guidelines

- **Security:** Implement industry-standard security practices, including encryption for sensitive data, secure authentication mechanisms, and input validation to prevent common vulnerabilities like SQL injection and cross-site scripting (XSS).
  
- **Error Handling:** Implement robust error handling mechanisms both on the client and server to provide meaningful error messages for users and developers.

- **Testing:** Conduct unit, integration, and end-to-end testing to ensure the reliability and functionality of the application. Utilize testing frameworks like Jest for server-side testing and Flutter's testing framework for client-side testing.

- **Documentation:** Document the codebase thoroughly, including inline comments, API documentation, and high-level system documentation, ensuring that developers can understand the codebase and its functionalities easily.

- **Scalability:** Design the system with scalability in mind, allowing for easy horizontal scaling of servers and efficient management of database connections.

- **Performance Optimization:** Profile and optimize critical parts of the application to ensure fast response times and a smooth user experience.

By adhering to these guidelines, Trove can be developed as a robust, secure, and efficient mobile application, meeting industry standards and user expectations.

// ========================
//      CODING STANDARDS
// ========================

// FILE NAMING:
// Use descriptive, PascalCase file names for classes and modules.
// For example, UserProfileService.ts

// VARIABLE NAMING:
// Use self-descriptive names for variables, functions, and classes.
// Choose names that clearly convey the purpose and usage of the code element.
// For example, use userProfileData instead of data or temp.
// Function names should indicate actions and start with a verb.
// For example, getUserProfile(), calculateTotalAmount().

// INDENTATION:
// Use 2 spaces for indentation. Avoid tabs.

// BRACES AND SPACING:
// Use braces for control structures (if, loops, functions) even for one-liners.
// Place opening braces on the same line as the control structure.
// Use a space after keywords like if, else, for, while.
// For example:
// if (condition) {
//     // code here
// } else {
//     // code here
// }

// COMMENTS:
// Use meaningful comments. Comments should explain why the code is doing something
// if the code isn't self-explanatory.
// For example, complex algorithms, important decisions, or workarounds.
// Avoid redundant comments that simply restate the code.
// Comment should be above the code it explains and indented at the same level as the code.

// ========================
//      END OF STANDARDS
// ========================
