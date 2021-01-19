C# | Namespaces

Namespaces are used to organise the classes. It helps to control the scope of methods and classes in larger .Net programming projects. In simpler words you can say that it provides a way to keep one set of names (like class names) different from other sets of names. The biggest advantage of using namespace is that the class names which are declared in one namespace will not clash with the same class names declared in another namespace. It is also referred as named group of classes having common features. The members of a namespace can be namespaces, interfaces, structures, and delegates.

Defining a Namespace

To define a namespace in C#, we will use the namespace keyword followed by the name of the namespace and curly braces containing the body of the namespace as follows:

Syntax:

namespace name_of_namespace {

  // Namespace (Nested Namespace)
  // Classes
  // Interfaces
  // Structures
  // Delegates

}

Example:

// defining the namespace name1
namespace name1
{

  // C1 is the class in the namespace name1 class C1
  {
    // class code
  }
}

Accessing the Members of Namespace

The members of a namespace are accessed by using dot(.) operator. A class in C# is fully known by its respective namespace.

Syntax:

[namespace_name].[member_name]

Note:

- Two classes with the same name can be created inside 2 different namespaces in a single program.
- Inside a namespace, no two classes can have the same name.
- In C#, the full name of the class starts from its namespace name followed by *dot(.)* operator and the class name, which is termed as the fully qualified name of the class.

Example:

// C# program to illustrate the use of namespaces

// namespace declaration
namespace first {

  // name_1 namespace members
  // i.e. class
  class Geeks_1
  {

    // function of class Geeks_1
    public static void display()
    {
      // Here System is the namespace under which Console class is defined, you can avoid writing System with the help of "using" keyword discussed later in this article
      System.Console.WriteLine("Hello Geeks!");
    }
  }

  // Removing comment will give the error because no two classes can have the same name under a single namespace

  class Geeks_1
  {

  }   // ending of first namespace

}

// Class declaration
class Geeks_2
{

  // Main Method
  public static void Main(String []args)
  {

    // calling the display method of class Geeks_1 by using two dot operator as one is used to access the class of first namespace and another is used to access the static method of class Geeks_1. Termed as fully qualified name

    first.Geeks_1.display();

  }
}
