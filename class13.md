## 1. Parent-Child Relationship
- Example: Teachers and Students
- Explanation: Teachers can have multiple students, but each student has one teacher for a specific subject.
## 2. One-to-Many Relationship
- Example: Teams and Players in sports
- Explanation: Each team can have multiple players, but each player belongs to one team at a time.
## 3. One-to-Many Relationship (Marbles Example)
- Example: Organizing marbles for yourself and a friend
- Explanation: You have your own group of favorite marbles ("One"), and your friend has a separate group ("Many") that you're helping to organize. Each group belongs to its respective owner.
## 4. Unit Testing vs. Integration Testing
- Unit Testing Scope: Testing individual code units (e.g., functions, methods, classes).
- - Isolation: Testing in isolation, often using mocks or stubs for dependencies.
- - Purpose: Ensures that small code units work correctly.
- - Speed: Fast, as it doesn't involve the entire application.
- - Detecting Bugs: Excellent for catching bugs within code units.
- Integration Testing
- - Scope: Testing interactions between different components or modules.
- - Real Dependencies: Uses real dependencies and external systems.
- - Purpose: Ensures integrated parts of the application work together.
- - Speed: Slower due to multiple components and setup.
- - Detecting Bugs: Uncovers issues related to data flow, interactions, and configuration.
## 5. Spring MVC Testing with MockMvc
- Usage: MockMvc is a tool for testing Spring MVC controllers.
- Set Up: Configure MockMvc within test methods or classes.
- Actions: Simulate HTTP requests (e.g., GET, POST) and configure request parameters.
- Assertions: Verify responses, including status codes, content, and headers.
## 6. How to Use MockMvc
- Simulate a Request: Use perform() to create and send an HTTP request.
- Send the Request: The request is sent to your application.
- Capture the Response: The response from your controller is captured.
- Assertion and Testing: Perform assertions on the response to check controller behavior.