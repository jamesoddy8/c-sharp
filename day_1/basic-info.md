Hello World in C#

The Hello World! program is the most basic and first program when you dive into a new programming language. This simply prints the Hello World! on the output screen. In C#, a basic program consists of the following:

* A Namespace declaration
* Class Declaration & Definition
* Class Members (like variables, methods, etc)
* Main Method
* Statements or Expressions

Example:

// C# program to print Hello World!
using System;

// namespace declaration
namespace HelloWorldApp {

  // Class declaration
  class Geeks {

    // Main method
    static void Main(string[] args) {

      // statement
      // printing Hello World!
      Console.WriteLine("Hello World!");

      // to prevent the screen from running an closing quickly
      Conole.ReadKey();
    }
  }
}
