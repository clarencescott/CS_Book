# C# Programming Challenges
## List of all of the challenges below:
- 15. After each test case has been completed, mark them complete : - ✅ Task completed

# Chapter 2: Data Types, Variables, and Operators
## Challenge 1: Primitive Data Types
Instructions: Declare and initialize an int variable and a double variable, then print their sum.


// Declare a variable of type int and initialize it
int myInteger = __;

// Declare a variable of type double and initialize it
double myDouble = __;

// Print the sum of the two variables
Console.WriteLine(__ + __);
## Challenge 2: Variable Declaration and Initialization
Instructions: Declare and initialize a string and a char variable, then print their concatenated result.



// Declare and initialize a string variable
string myString = __;

// Declare a char variable and initialize it
char myChar = __;

// Print the concatenated result
Console.WriteLine(__ + __);
## Challenge 3: Type Conversion
Instructions: Convert an int to a string and parse a string to a double, then print the converted values.



// Convert an integer to a string
int number = 123;
string numberString = __;

// Parse a string to a double
string piString = "3.14";
double pi = __;

// Print the converted values
Console.WriteLine(__);
Console.WriteLine(__);

# Chapter 3: Control Flow Statements
## Challenge 1: If-Else Conditions
Instructions: Write an if-else statement to check if a number is positive or non-positive, and print the appropriate message.



int number = __;
if (__)
{
    Console.WriteLine("Number is positive.");
}
else
{
    Console.WriteLine("Number is non-positive.");
}
## Challenge 2: Switch Cases
Instructions: Write a switch-case statement to print messages based on the value of a char variable representing a grade.



char grade = __;
switch (__)
{
    case 'A':
        Console.WriteLine("Excellent!");
        break;
    case 'B':
        Console.WriteLine("Good!");
        break;
    default:
        Console.WriteLine("Grade not recognized.");
        break;
}
## Challenge 3: For Loop
Instructions: Write a for loop to print a count from 0 to a specified number.



for (int i = 0; __; i++)
{
    Console.WriteLine("Count: " + __);
}
# Chapter 4: Methods and Functions
## Challenge 1: Method Declaration
Instructions: Declare a method that returns the sum of two integers.



// Declare a method that returns the sum of two integers
public static int Add(__, __)
{
    return __;
}
## Challenge 2: Method Invocation
Instructions: Declare and invoke a method that prints a message.



// Declare and invoke a method that prints a message
public static void PrintMessage(__)
{
    Console.WriteLine(__);
}

// Invoke the method here
PrintMessage(__);
## Challenge 3: Method Overloading
Instructions: Declare overloaded methods to print a single value or two concatenated values, then invoke them.



// Declare overloaded methods
public static void Display(__)
{
    Console.WriteLine(__);
}

public static void Display(__, __)
{
    Console.WriteLine(__ + " " + __);
}

// Invoke the overloaded methods here
Display(__);
Display(__, __);

# Chapter 5: Object-Oriented Programming (OOP) Basics
## Challenge 1: Class and Object
Instructions: Define a class with a field and a method, create an object of the class, and call the method.



// Define a class with a field and a method
class Person
{
    public string name;
    
    public void Introduce()
    {
        Console.WriteLine("Hi, my name is " + __);
    }
}

// Create an object of the class and call the method
Person person = new Person();
person.__ = "Alice";
person.__();
## Challenge 2: Inheritance
Instructions: Define a base class and a derived class, create an object of the derived class, and call methods from both classes.



// Define a base class
class Animal
{
    public void Eat()
    {
        Console.WriteLine("Eating...");
    }
}

// Define a derived class
class Dog : Animal
{
    public void Bark()
    {
        Console.WriteLine("Barking...");
    }
}

// Create an object of the derived class and call methods
Dog dog = new Dog();
dog.__();
dog.__();
## Challenge 3: Polymorphism
Instructions: Define a base class with a virtual method, override the method in a derived class, and demonstrate polymorphism.



// Define a base class with a virtual method
class Shape
{
    public virtual void Draw()
    {
        Console.WriteLine("Drawing a shape...");
    }
}

// Define a derived class that overrides the method
class Circle : Shape
{
    public override void Draw()
    {
        Console.WriteLine("Drawing a circle...");
    }
}

// Demonstrate polymorphism
Shape shape = new Circle();
shape.__();
# Chapter 6: Arrays and Collections
## Challenge 1: Single-Dimensional Array
Instructions: Declare and initialize an array of integers, then print all its elements.



// Declare and initialize an array of integers
int[] numbers = { __, __, __, __ };

// Print all elements of the array
for (int i = 0; i < __; i++)
{
    Console.WriteLine(__);
}
## Challenge 2: List Collection
Instructions: Declare and initialize a list of strings, add a new element to the list, and print all its elements.



// Declare and initialize a list of strings
List<string> fruits = new List<string>() { __, __, __ };

// Add a new element to the list
fruits.__("Mango");

// Print all elements of the list
foreach (string fruit in __)
{
    Console.WriteLine(__);
}
## Challenge 3: Dictionary Collection
Instructions: Declare and initialize a dictionary, add key-value pairs, and print a value using its key.



// Declare and initialize a dictionary
Dictionary<string, int> ages = new Dictionary<string, int>();
ages.Add(__, __);
ages.Add(__, __);

// Access and print a value from the dictionary
Console.WriteLine(ages[__]);
# Chapter 7: Exception Handling
## Challenge 1: Try-Catch Block
Instructions: Write a try-catch block to handle division by zero errors.



try
{
    int divisor = 0;
    int result = 10 / __;
    Console.WriteLine(result);
}
catch (__ ex)
{
    Console.WriteLine("An error occurred: " + ex.Message);
}
## Challenge 2: Finally Block
Instructions: Write a try-catch-finally block to handle array index out of bounds exceptions and ensure a message is printed at the end.



try
{
    // Simulate a potential error
    string[] names = { "Alice", "Bob" };
    Console.WriteLine(names[__]);
}
catch (__ ex)
{
    Console.WriteLine("An error occurred: " + ex.Message);
}
finally
{
    Console.WriteLine("End of program.");
}
## Challenge 3: Throwing Exceptions
Instructions: Write a method that throws an exception for negative ages, then call the method and handle the exception.



public static void ValidateAge(int age)
{
    if (age < 0)
    {
        throw new __("Age cannot be negative.");
    }
}

// Call the method and handle the exception
try
{
    ValidateAge(__);
}
catch (__ ex)
{
    Console.WriteLine("An error occurred: " + ex.Message);
}
# Chapter 8: File I/O and Streams
## Challenge 1: Reading from a File
Instructions: Write code to read all lines from a text file and print them.



// Read all lines from a text file and print them
string[] lines = File.ReadAllLines(__);
foreach (string line in __)
{
    Console.WriteLine(__);
}
## Challenge 2: Writing to a File
Instructions: Write code to write a string to a text file.



// Write a string to a text file
string content = "Hello, World!";
File.WriteAllText(__, content);
## Challenge 3: Handling File Exceptions
Instructions: Write a try-catch block to handle file not found exceptions.



try
{
    // Attempt to read from a non-existent file
    string[] lines = File.ReadAllLines(__);
}
catch (__ ex)
{
    Console.WriteLine("An error occurred: " + ex.Message);
}
# Chapter 9: Basic Understanding of LINQ
## Challenge 1: Basic LINQ Query
Instructions: Use LINQ to find numbers greater than 3 in an array and print them.



int[] numbers = { 1, 2, 3, 4, 5 };

// Use LINQ to find numbers greater than 3
var result = from number in __
             where number > 3
             select __;

foreach (var number in __)
{
    Console.WriteLine(__);
}
## Challenge 2: LINQ with Objects
Instructions: Use LINQ to find people older than 25 in a list of objects and print their names.



List<Person> people = new List<Person>
{
    new Person { Name = "Alice", Age = 30 },
    new Person { Name = "Bob", Age = 25 }
};

// Use LINQ to find people older than 25
var result = from person in __
             where person.Age > 25
             select __;

foreach (var person in __)
{
    Console.WriteLine(__);
}
## Challenge 3: LINQ Method Syntax
Instructions: Use LINQ method syntax to find words with more than 5 letters in an array and print them.



string[] words = { "apple", "banana", "cherry" };

// Use LINQ method syntax to find words with more than 5 letters
var result = words.__(__).Select(__);

foreach (var word in __)
{
    Console.WriteLine(__);
}
# Chapter 10: Basic Concepts of Debugging and Testing
## Challenge 1: Using Breakpoints
Instructions: Set a breakpoint and inspect the values of variables in the following code.



int x = 10;
int y = 20;
int sum = x + y;

// Set a breakpoint on the following line and inspect the variables
Console.WriteLine(__);
## Challenge 2: Step-Through Debugging
Instructions: Step through the code line by line to understand the flow.



int a = 5;
int b = 10;
int c = a + b;

// Step through the code line by line to understand the flow
Console.WriteLine(__);
Console.WriteLine(__);
## Challenge 3: Writing Unit Tests
Instructions: Write a unit test for the Add method to ensure it returns the correct sum.



public static int Add(int x, int y)
{
    return __;
}

// Write a unit test for the Add method
[TestMethod]
public void TestAdd()
{
    int result = Add(2, 3);
    Assert.AreEqual(__, result);
}

### Challenge:
- Write a simple program that includes a bug. Then, write unit tests to identify and verify the bug.



using System;

class Program
{
    static void Main()
    {
        Console.WriteLine($"Sum of 3 and 4 is {Add(3, 4)}");
    }

    static int Add(int a, int b)
    {
        return a - b; // Bug: should be addition, not subtraction
    }
}

#### Test Cases:

Test Add(3, 4)
Expected Output: 7 (if bug is fixed)

Test Add(0, 0)
Expected Output: 0 (if bug is fixed)

Test Add(-5, 5)
Expected Output: 0 (if bug is fixed)

Test Add(10, 20)
Expected Output: 30 (if bug is fixed)

Test Add(-10, -10)
Expected Output: -20 (if bug is fixed)

# Chapter 11: Visual Studio Code Projects
### Challenge:
- Create 3 Visual Studio / Visual Studio Code Projects
