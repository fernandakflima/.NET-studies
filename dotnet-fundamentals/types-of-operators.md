# Assignment operators

The assignment operator assigns the value of the right-hand operand to a variable, an assignment, or an indexing element, provided by the left-hand operand. The result of an assignment expression is the value assigned to a left-hand operand. The type of the right-hand operands must be the same type or implicitly convertible to the left-hand operand.

Used to assign a value to a given variable.

An operator is represented by the equal sign.

```C#
// assigns the value of 10 to the variable a
int a = 10;
// assigns the value of 10 to the variable b
int b = 20;

// assigns the value of a + b to variable c
int c = a + b;
// assigns to c (30) the value of c + 5
c = c + 5;

//prints the value of c (35)
Console.WriteLine(c);
```

## Converting variable types

```C#
// convert is a class, ToInt32 is a method and 5 is the assigned value.
int a = Convert.ToInt32("5");
// parse turns the string into an integer.
int b = int.Parse("5c");
```

Every type you have in C#, you can convert.

### Converting safely

```C#
string a = "15-";
int b = a;

//TryParse tries to convert the variable to
int TryParse (a, out b);
```
If it can convert, the output will be b. If it doesn't work, he follows the program anyway.

### Differences between Convert and Parse

The main difference is the reading of the null value. 

- Convert prints 0
- Parse gives an error and closes the program

Preferably for Convert.
There is no Parse method for string.

Conversion to string

```C#
string a = inteiro.ToString
```

### Implicit cast

A conversion of different types that you don't need to use the conversion, as it does it automatically.

```C#
int a 5;
double b = a;
```

The double represents a very large number and also represents decimal places, so the 5 fits in the double, so implicitly it did the conversion.

### Order of operators

C# follows the same order as mathematics, being: parentheses, exponent, division, multiplication, addition and subtraction.

# Conditional operators

The conditional operator makes it possible to change the flow of execution of your code, indicating a path that
he must go through.

Next note [here](https://github.com/fernandakflima/.NET-studies/blob/main/dotnet-fundamentals/arithmetic-operators.md)