# C# Programming Challenges
## List of all of the challenges below:
- 15. After each test case has been completed, mark them complete : - ✅ Task completed

# Chapter 2: Data Types, Variables, and Operators - ✅ Task completed
### Challenge:
- Write a program that performs basic arithmetic operations (addition, subtraction, multiplication, and division) on two numbers provided by the user. The program should display the results of these operations.
*** Updated the code to remove the console read line inputs and take them as declared/initilized variables. ***
*** Changed the code to include one test case that does not use the variables declared and initilized. ***


using System;

class Program
{
    static void Main()
    {

        Console.WriteLine($"Addition: {num1 + num2}");
        Console.WriteLine($"Subtraction: {num1 - num2}");
        Console.WriteLine($"Multiplication: {  *  }");
        Console.WriteLine($"Division: {num1 / num2}");
    }
}

#### Test Cases:
##### Solutions
- int num1 = 10;
- int num2 = 5;
###### Multiplication
- Console.WriteLine($"Multiplication: {49 * 2}");

Input: 10, 5
Expected Output:
Addition: 15
Subtraction: 5
Multiplication: 98
Division: 2


##### Solutions
- int num1 = 7;
- int num2 = 3;
###### Division
-Console.WriteLine($"Division: {(float)num1 / (float)num2}");

Input: 7, 3
Expected Output:
Addition: 10
Subtraction: 4
Multiplication: 21
Division: 2.333

##### Solutions
- int num1 = 0;
- int num2 = 5;

Input: 0, 5
Expected Output:
Addition: 5
Subtraction: -5
Multiplication: 0
Division: 0

##### Solutions
- int num1 = -10;
- int num2 = 5;

Input: -10, 5
Expected Output:
Addition: -5
Subtraction: -15
Multiplication: -50
Division: -2

##### Solutions
- int num1 = 10;
- int num2 = 0;

###### Division
Unhandled exception. System.DivideByZeroException: Attempted to divide by zero.
Input: 10, 0
Expected Output:
Addition: 10
Subtraction: 10
Multiplication: 0
Division: Infinity (or handle division by zero)

# Chapter 3: Control Flow Statements
### Challenge:
- Write a program that takes an integer input from the user and determines if it is positive, negative, or zero using if-else statements. Additionally, use a loop to repeatedly prompt the user until they enter a valid number.



using System;

class Program
{
    static void Main()
    {
        int number;
        bool validInput = false;

        while (!validInput)
        {
            Console.Write("Enter an integer: ");
            validInput = int.TryParse(Console.ReadLine(), out number);

            if (validInput)
            {
                if (number > 0)
                    Console.WriteLine("The number is positive.");
                else if (number < 0)
                    Console.WriteLine("The number is negative.");
                else
                    Console.WriteLine("The number is zero.");
            }
            else
                Console.WriteLine("Invalid input, please enter an integer.");
        }
    }
}

#### Test Cases:

Input: 10
Expected Output: The number is positive.

Input: -5
Expected Output: The number is negative.

Input: 0
Expected Output: The number is zero.

Input: "abc" (multiple attempts with invalid input before a valid number)
Expected Output: Invalid input, please enter an integer. (repeatedly)
After a valid number is entered, output as per the valid input.

Input: 999
Expected Output: The number is positive.

# Chapter 4: Methods and Functions
### Challenge:
- Write a program that defines a method to calculate the factorial of a given number. Use this method to compute the factorial of numbers provided by the user.



using System;

class Program
{
    static void Main()
    {
        Console.Write("Enter a number to calculate its factorial: ");
        int number = Convert.ToInt32(Console.ReadLine());
        
        if (number < 0)
            Console.WriteLine("Factorial is not defined for negative numbers.");
        else
            Console.WriteLine($"The factorial of {number} is {Factorial(number)}");
    }

    static long Factorial(int n)
    {
        if (n == 0)
            return 1;
        return n * Factorial(n - 1);
    }
}

#### Test Cases:

Input: 5
Expected Output: The factorial of 5 is 120.

Input: 0
Expected Output: The factorial of 0 is 1.

Input: 7
Expected Output: The factorial of 7 is 5040.

Input: 10
Expected Output: The factorial of 10 is 3628800.

Input: -3
Expected Output: Factorial is not defined for negative numbers.

# Chapter 5: Object-Oriented Programming (OOP) Basics
### Challenge:
- Create a simple Person class with properties for Name and Age. Write a program to create an instance of this class, set the properties, and display the person's information.



using System;

class Person
{
    public string Name { get; set; }
    public int Age { get; set; }

    public void DisplayInfo()
    {
        Console.WriteLine($"Name: {Name}");
        Console.WriteLine($"Age: {Age}");
    }
}

class Program
{
    static void Main()
    {
        Person person = new Person();
        person.Name = "Alice";
        person.Age = 30;
        person.DisplayInfo();
    }
}

#### Test Cases:

Name: Alice, Age: 30
Expected Output:
Name: Alice
Age: 30

Name: Bob, Age: 25
Expected Output:
Name: Bob
Age: 25

Name: Charlie, Age: 40
Expected Output:
Name: Charlie
Age: 40

Name: Diana, Age: 22
Expected Output:
Name: Diana
Age: 22

Name: Eve, Age: 50
Expected Output:
Name: Eve
Age: 50

# Chapter 6: Arrays and Collections
### Challenge:
- Write a program that initializes an array of integers, sorts it, and prints the sorted array.



using System;

class Program
{
    static void Main()
    {
        int[] numbers = { 5, 3, 8, 1, 2 };
        
        Array.Sort(numbers);
        
        Console.WriteLine("Sorted array:");
        foreach (int number in numbers)
        {
            Console.Write(number + " ");
        }
    }
}

#### Test Cases:

Array: {5, 3, 8, 1, 2}
Expected Output: Sorted array: 1 2 3 5 8

Array: {10, 20, 5, 15}
Expected Output: Sorted array: 5 10 15 20

Array: {7, 3, 9, 0}
Expected Output: Sorted array: 0 3 7 9

Array: {12, 45, 7, 32}
Expected Output: Sorted array: 7 12 32 45

Array: {100, 2, 9, 40, 75}
Expected Output: Sorted array: 2 9 40 75 100

# Chapter 7: Exception Handling
### Challenge:
- Write a program that reads a number from the user and divides 100 by that number. Handle any potential exceptions such as division by zero and invalid input.



using System;

class Program
{
    static void Main()
    {
        try
        {
            Console.Write("Enter a number: ");
            int number = Convert.ToInt32(Console.ReadLine());

            double result = 100 / number;
            Console.WriteLine($"Result: {result}");
        }
        catch (DivideByZeroException)
        {
            Console.WriteLine("Error: Division by zero is not allowed.");
        }
        catch (FormatException)
        {
            Console.WriteLine("Error: Invalid input format.");
        }
        catch (Exception ex)
        {
            Console.WriteLine($"Error: {ex.Message}");
        }
    }
}

#### Test Cases:

Input: 10
Expected Output: Result: 10

Input: 0
Expected Output: Error: Division by zero is not allowed.

Input: "abc"
Expected Output: Error: Invalid input format.

Input: 50
Expected Output: Result: 2

Input: 100
Expected Output: Result: 1

# Chapter 8: File I/O and Streams
### Challenge:
- Write a program that reads text from a file and displays its contents. Create a file with some text and test the program.



using System;
using System.IO;

class Program
{
    static void Main()
    {
        string path = "example.txt";
        
        try
        {
            string content = File.ReadAllText(path);
            Console.WriteLine("File contents:");
            Console.WriteLine(content);
        }
        catch (FileNotFoundException)
        {
            Console.WriteLine("Error: File not found.");
        }
        catch (IOException ex)
        {
            Console.WriteLine($"Error: {ex.Message}");
        }
    }
}

#### Test Cases:

File Exists: Contains "Hello World!"
Expected Output: File contents: Hello World!

File Exists: Contains "C# Programming"
Expected Output: File contents: C# Programming

File Does Not Exist
Expected Output: Error: File not found.

File Exists: Contains "This is a test file."
Expected Output: File contents: This is a test file.

File Exists: Contains "Data from file I/O test."
Expected Output: File contents: Data from file I/O test.

# Chapter 9: Basic Understanding of LINQ
### Challenge:
- Write a program that uses LINQ to filter a list of integers, returning only those greater than 10 and sorting them in ascending order.



using System;
using System.Linq;
using System.Collections.Generic;

class Program
{
    static void Main()
    {
        List<int> numbers = new List<int> { 5, 12, 7, 15, 1, 20 };

        var filteredNumbers = numbers.Where(n => n > 10).OrderBy(n => n);

        Console.WriteLine("Filtered and sorted numbers:");
        foreach (var number in filteredNumbers)
        {
            Console.Write(number + " ");
        }
    }
}

#### Test Cases:

List: {5, 12, 7, 15, 1, 20}
Expected Output: Filtered and sorted numbers: 12 15 20

List: {1, 2, 3, 4, 5}
Expected Output: Filtered and sorted numbers:

List: {30, 25, 10, 35, 40}
Expected Output: Filtered and sorted numbers: 25 30 35 40

List: {50, 12, 7, 18}
Expected Output: Filtered and sorted numbers: 12 18 50

List: {20, 30, 15, 5, 25}
Expected Output: Filtered and sorted numbers: 15 20 25 30

# Chapter 10: Basic Concepts of Debugging and Testing
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
