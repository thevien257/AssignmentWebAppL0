# Milestone 01: Hello World

## **Introduction**

This milestone aims to set up the foundational environment for developing a web application and application server. The milestone's deliverables include a functional "Hello World" web page and a server that prints "Hello World" to the console.

## **Project Overview**

The project involves developing a web application using ReactJS and a server using Spring Boot. The following steps were completed during this milestone:

1. Setting up the development environment.
2. Creating a ReactJS project to display a "Hello World" page.
3. Setting up a Spring Boot server to print "Hello World" to the console.

---

## **Setup Instructions**

### **1. Development Environment**

- **Operating System:** Windows
- **Tools Installed:**
  - Node.js (v18.x)
  - npm (v8.x)
  - IntelliJ IDEA (for Spring Boot development)
  - Postman (for API testing)

### **2. Web Application**

1. Created a ReactJS project using the following command:

   ```bash
   npx create-react-app hello-world-app
   ```

2. Updated the `App.js` file to display "Hello World":

   ```jsx
   import React from "react";

   function App() {
     return (
       <div className="App">
         <h1>Hello, World!</h1>
       </div>
     );
   }

   export default App;
   ```

3. Ran the development server:
   ```bash
   npm start
   ```
   - The "Hello World" page was successfully displayed at `http://localhost:3000`.

### **3. Application Server**

1. Set up a Spring Boot project:

   - Initialized a new Spring Boot project using [Spring Initializr](https://start.spring.io/).
   - Included dependencies for Web and Spring Boot DevTools.

2. Implemented a basic controller to print "Hello World":

   ```java
   import org.springframework.web.bind.annotation.GetMapping;
   import org.springframework.web.bind.annotation.RestController;

   @RestController
   public class HelloWorldController {

       @GetMapping("/hello")
       public String sayHello() {
           System.out.println("Hello, World!");
           return "Hello, World!";
       }
   }
   ```

3. Ran the application and verified that "Hello World" was printed to the console.

---

## **Deliverables**

1. **Web Application:**

   - A ReactJS-based web app displaying "Hello World."
   - Screenshot of the web page.

2. **Application Server:**

   - A Spring Boot application running successfully.
   - Screenshot of the console output displaying "Hello World."

3. **Video Report:**
   - [Demonstration Video](https://drive.google.com/file/d/1ujR9kjJjv37AltEZ2M3IAZ8FiXKAXi5A/view?usp=sharing)

---

## **Conclusion**

Milestone 01 was successfully completed with the following deliverables:

- A working "Hello World" web application and server.
- A demonstration video showcasing the implementation.

The foundational setup is now ready for further development in subsequent milestones.
