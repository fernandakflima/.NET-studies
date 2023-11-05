# Syntax and Indentation

When starting the C# project, with the 'dotnet new console' command, it originally creates some folders:

**bin** - this folder contains the binary file

**obj** - this folder contains bug files, when you compile the code, it will generate files that will be sent to this folder.

FileName.csproj - **.csproj** is a C# project file, in it, contains some essential information that is descriptive for the project. It is known as meta data and uses XML language: <></>

Program.cs - **Program** is the name of your class; **.cs** identification that it is a C# file

## The concept of class

The class is related to the concept of abstraction in object-oriented programming.

**Abstraction:** An abstraction is that you take an object in real life and transform it into another object in programming, so that you can enter it and implement your actions.

**Method:** It is an action that your class will do.

**Class:** It would be your "object".

**Attributes:** Data such as name, age, etc.

When you represent a class, first it has its attributes, then its methods.

The class represents a mold, it represents the construction of an object.

The concretization of the class is the object.

## Exploring the syntax

Person.cs file: is the class I created

```C#
// namespace is an organization of classes
namespace ExampleFundamentals.Models
{
    public class Person
    {
        public string Name { get; set; }
        public int Age { get; set; }

        public void Introduce()
        {
            //the $ sign calls the attributes to the Console
            Console.WriteLine($"Hello, my name is {Name}, and I'm {Age} years old.")
        }
    }
}
```

Program.cs file: it is the project input, so all actions will be done in the Program. It is through the NameSpace that the Program recognizes paths and classes.

**Models** is the folder I created to store my classes.

```C#
using ExampleFundamentals.Models

Person personOne = new Person();

// the . means a continuation of an action
personOne.Name = "Kali";
personOne.Age = 24;
personOne.Introduce();
```

## Case conventions

**Case** is a writing pattern.

- camelCase;
- PascalCase;
- snake_case;
- spinal-case

In C# we use camelCase and PascalCase

### Case conventions in code

There is no obligation to follow this pattern, the code will run the same way, however, it is good to follow this pattern to maintain clean code that is easy to read and maintain.

- To name classes, use PascalCase;
- To name properties, use PascalCase;
- To name method, use Pascalcase
- To name variable, use camelCase

### Class writing convention

It's not recommended to abbreviate variable names.

The file name must match the name of your class.

person.cs file, person class; This makes it easier to read and find.

### Variable name convention

Must not contain special characters, other than underline, in variables, properties and classes.

## Data types

| Type | Represents | Range | Default Value |
|------|------------|-------|---------------|
| string | A series of characters | | |
| char | A Unicode character | | |
| object | Object type | | |
| bool | Boolean value | True of False | False |
| byte | 8-bit unsigned integer | 0 to 255 | 0 |
| decimal | decimal values with 28-29 significant digits | (+ or -) 1.0 x 10e-28 to 7.9 x 10e28 | 0.0M |
| double | 64 bit double-precision floating point type | (+/-) 5.0 x 10 raise to -324 to (+/-) 1.7 x 10 raise to 308 | 0.0D |
| int | 32 bit signed integer type | -2,147,483,648 to 2,147,483,647 | 0 |
| float | 32 bit single-precision floating point type | -3.4 x raise to 38 to + 3.4 x 10 raise to 38 | 0.0F |
| long | 64 bit signed integer type | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | OL |
| uint | 32 bit unsigned integer type | 0 to 4,294,967,295 | 0 |
| short | 16 bit signed integer type | -32,768 to 32,767 | 0 |
| ulong | 64 bit unsigned integer type | 0 to 18,446,744,073,709,551,615 | 0 |

## Manipulating variables

**Scope** is a piece of block that you will carry out your codes in - usually it is the beginning and end of a brace, {}.

**DataTime** is a way to represent dates in C#

Next note [here](https://github.com/fernandakflima/.NET-studies/blob/main/dotnet-fundamentals/types-of-operators.md)