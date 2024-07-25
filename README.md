# C Sharp Book

## Details

- Each chapter from the C# Basics to Advanced book I wrote will be overviewed in here
- Each overview will come with: Title of Chapter, Detail of what was covered in the chapter, Example code (console(terminal) or WPF/Desktop Application).
- There will be 2 chapters being skipped: Intro to C# & Intro to Visual Studio.
- There will be 5 test cases in each application type to cover key concepts.
- Although Intro to Visual Studio will be skipped, I will still build the needed applications through Visual Studio. I will cover this more once I have them decided.
- Each chapter will get a new folder to hold the contents needed in later projects:
> .Net: New Project > Project Template > Save Location > Create Project

# Rules

1. Read and fully understand the problem you are trying to solve.
Understand the Problem Statement
Break down the problem into smaller, manageable tasks.
Plan Before Coding

2. Outline the structure of your application.
Create a flowchart or pseudocode to map out the logic.
Identify the main classes, methods, and data structures you will use.
Follow Best Practices

3. Use meaningful variable and method names.
Keep methods short and focused on a single task.
Avoid using magic numbers; use constants or enums instead.
Write Clean Code

4. Adhere to the SOLID principles.
Ensure your code is readable and maintainable.
Use comments to explain complex logic but avoid over-commenting.
Use Version Control

5. Commit your code regularly with meaningful commit messages.
Use branches to experiment with new features or changes.
Error Handling

6. Implement proper error handling using try-catch blocks.
Validate inputs to prevent errors and improve security.
Log errors for easier debugging and maintenance.
Testing

7. Write unit tests for your code to ensure functionality.
Use test-driven development (TDD) where applicable.
Test edge cases and handle potential exceptions.
Code Reviews

8. Review your code before considering it complete.
Use tools like linters or static code analyzers to identify potential issues.
Seek feedback from peers or mentors if possible.
Refactoring

9. Regularly refactor your code to improve structure and readability.
Simplify complex code without changing functionality.
Eliminate redundant or duplicate code.
Documentation

10. Document your code, especially public APIs and complex logic.
Create user guides or readme files to explain how to use your application.
Update documentation regularly to reflect code changes.
Performance Optimization

11. Profile your code to identify bottlenecks.
Optimize algorithms and data structures for efficiency.
Avoid premature optimization; focus on critical parts of the code.
Security

12. Follow secure coding practices to protect against vulnerabilities.
Sanitize inputs to prevent injection attacks.
Use encryption for sensitive data.
Consistency

13. Stick to a consistent coding style throughout your project.
Use a style guide or coding standards document.
Ensure consistency in naming conventions, indentation, and formatting.
Learning and Improvement

14. Reflect on what you’ve learned after completing each application.
Identify areas for improvement and set goals for the next chapter.
Stay updated with the latest C# features and best practices.

15. After each chapter has been completed, mark them complete : - ✅ Task completed

# Topcis
## Chapter 1: Intro to C#:
- Creating a program that prints out "Welcome to my C# Programming Portfolio!"

## Chapter 2: Data Types, Variables, and Operators

## Chapter 3: Control Flow Statements 

## Chapter 4: Methods and Functions 

## Chapter 5: Object-Oriented Programming (OOP) 

## Chapter 6: Arrays and Collections 

## Chapter 7: Exception Handling 

## Chapter 8: File I/O and Streams 

## Chapter 9: Basic Understanding of LINQ

## Chapter 10: Basic Concepts of Debugging and Testing

## Chapter 11: Visual Studio Code Projects


# C# Book Challenge Checklist

#### Understanding and Planning
- [ ] Read and fully understand the problem statement.
- [ ] Break down the problem into smaller, manageable tasks.
- [ ] Outline the structure of your application.
- [ ] Create a flowchart or pseudocode to map out the logic.
- [ ] Identify the main classes, methods, and data structures to use.

#### Coding Best Practices
- [ ] Use meaningful variable and method names.
- [ ] Keep methods short and focused on a single task.
- [ ] Avoid using magic numbers; use constants or enums instead.

#### Writing Clean Code
- [ ] Adhere to the SOLID principles.
- [ ] Ensure code is readable and maintainable.
- [ ] Use comments to explain complex logic, avoiding over-commenting.

#### Version Control
- [ ] Commit code regularly with meaningful commit messages.
- [ ] Use branches to experiment with new features or changes.

#### Error Handling
- [ ] Implement proper error handling using try-catch blocks.
- [ ] Validate inputs to prevent errors and improve security.
- [ ] Log errors for easier debugging and maintenance.

#### Testing
- [ ] Write unit tests for your code to ensure functionality.
- [ ] Use test-driven development (TDD) where applicable.
- [ ] Test edge cases and handle potential exceptions.

#### Code Reviews
- [ ] Review your code before considering it complete.
- [ ] Use tools like linters or static code analyzers to identify potential issues.
- [ ] Seek feedback from peers or mentors if possible.

#### Refactoring
- [ ] Regularly refactor code to improve structure and readability.
- [ ] Simplify complex code without changing functionality.
- [ ] Eliminate redundant or duplicate code.

#### Documentation
- [ ] Document code, especially public APIs and complex logic.
- [ ] Create user guides or readme files to explain how to use the application.
- [ ] Update documentation regularly to reflect code changes.

#### Performance Optimization
- [ ] Profile code to identify bottlenecks.
- [ ] Optimize algorithms and data structures for efficiency.
- [ ] Avoid premature optimization; focus on critical parts of the code.

#### Security
- [ ] Follow secure coding practices to protect against vulnerabilities.
- [ ] Sanitize inputs to prevent injection attacks.
- [ ] Use encryption for sensitive data.

#### Consistency
- [ ] Stick to a consistent coding style throughout the project.
- [ ] Use a style guide or coding standards document.
- [ ] Ensure consistency in naming conventions, indentation, and formatting.

#### Learning and Improvement
- [ ] Reflect on what you’ve learned after completing each application.
- [ ] Identify areas for improvement and set goals for the next chapter.
- [ ] Stay updated with the latest C# features and best practices.


# C# Style Guide and Coding Standards

## 1. Naming Conventions
### 1.1 General Naming Rules
- Use meaningful and descriptive names.
- Avoid abbreviations, except for widely understood acronyms (e.g., `HTML`, `XML`).

### 1.2 Classes and Interfaces
- **Classes**: Use PascalCase (e.g., `CustomerOrder`, `Employee`).
- **Interfaces**: Prefix with `I` and use PascalCase (e.g., `IOrderProcessor`, `IEmployee`).

### 1.3 Methods
- Use PascalCase (e.g., `CalculateTotal`, `GetEmployeeDetails`).
- Use verbs or verb phrases to indicate actions.

### 1.4 Variables and Fields
- **Local variables and method parameters**: Use camelCase (e.g., `totalAmount`, `employeeName`).
- **Private fields**: Prefix with an underscore and use camelCase (e.g., `_totalAmount`, `_employeeName`).
- **Public fields**: Use PascalCase (e.g., `TotalAmount`, `EmployeeName`).

### 1.5 Constants
- Use PascalCase (e.g., `MaxValue`, `DefaultTimeout`).

### 1.6 Enums
- Use PascalCase for enum types and members (e.g., `enum OrderStatus { Pending, Completed, Canceled }`).

## 2. Code Layout and Formatting
### 2.1 Indentation
- Use 4 spaces for indentation. Do not use tabs.

### 2.2 Braces
- Place opening braces on the same line as the declaration, and closing braces on a new line.

```csharp
public void ExampleMethod()
{
    if (condition)
    {
        // Code here
    }
    else
    {
        // Code here
    }
}
```

### 2.3 Line Length
- Keep lines to a maximum of 80 characters when possible. Break long lines appropriately.

### 2.4 Spacing
- Use a single space around operators (e.g., `x = y + z;`).
- Do not add spaces after the opening parenthesis or before the closing parenthesis (e.g., `if (condition)`, not `if ( condition )`).

## 3. Commenting
### 3.1 Inline Comments
- Use inline comments sparingly. Place them on a new line above the code block they refer to.

### 3.2 XML Documentation Comments
- Use XML comments for public classes and methods.


## 4. Coding Best Practices
### 4.1 SOLID Principles
- Follow the SOLID principles to ensure code is modular, flexible, and easy to maintain.

### 4.2 DRY (Don't Repeat Yourself)
- Avoid code duplication. Use methods or classes to encapsulate repetitive logic.

### 4.3 KISS (Keep It Simple, Stupid)
- Keep your code simple and straightforward. Avoid unnecessary complexity.

### 4.4 YAGNI (You Aren't Gonna Need It)
- Implement functionality only when it is needed. Avoid speculative generality.

## 5. Error Handling
### 5.1 Try-Catch Blocks
- Use try-catch blocks to handle exceptions gracefully.

### 5.2 Custom Exceptions
- Use custom exceptions to represent specific error conditions.

## 6. Testing
### 6.1 Unit Tests
- Write unit tests for all public methods and classes using a testing framework like NUnit or MSTest.

### 6.2 Test Coverage
- Aim for high test coverage, but prioritize quality and meaningful tests over coverage percentage.

## 7. Version Control
### 7.1 Commit Messages
- Write clear and concise commit messages that describe the change.

### 7.2 Branching
- Use branches for new features, bug fixes, or experiments. Follow a branching strategy like Git Flow.

## 8. Refactoring
### 8.1 Regular Refactoring
- Regularly refactor code to improve structure, readability, and performance without changing functionality.

## 9. Performance Optimization
### 9.1 Profiling
- Profile code to identify performance bottlenecks and optimize critical sections.

## 10. Security
### 10.1 Input Validation
- Validate all inputs to prevent injection attacks and ensure data integrity.

### 10.2 Encryption
- Use encryption to protect sensitive data.

## 11. Consistency
### 11.1 Style Guide
- Stick to this style guide throughout the project to maintain consistency.

## 12. Learning and Improvement
### 12.1 Continuous Learning
- Stay updated with the latest C# features, tools, and best practices.
- Reflect on completed projects and identify areas for improvement.