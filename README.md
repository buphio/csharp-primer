# C# Primer

Short primer to quickly refresh my memory if needed.

## Table of Contents

- [Microsoft C# Coding Convetions](#microsft-c-coding-conventions)
- [Common Value Types](#common-value-types)
- [Strings](#strings)
- [Variables](#variables)

<br />

## Microsft C# Coding Conventions

[Microsft C# Coding Conventions](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/coding-style/coding-conventions)

## Common Value Types

| Type | Range | Size | .NET type |
|---|---|---|---|
| **byte** | 0 to 255 | 1 byte | System.Byte |
| **int**  | -2,147,483,648 to 2,147,483,647 | 4 bytes | System.Int32 |
| **long** | -9,223,372,036,854,775,808 to 9,223,372,036,854,775,807 | 8 bytes | System.Int64 |
| **float** | ±1.5 x 10e−45 to ±3.4 x 10e38 | 4 bytes | System.Single |
| **double** | ±5.0 × 10e−324 to ±1.7 × 10e308 | 8 bytes | System.Double |
| **bool** | | 1 bit | System.Boolean |
| **char** | U+0000 to U+FFFF | 2 bytes | System.Char |

## Strings

`string` represents a sequence of one or more Unicode characters. It is an alias for `System.String`.

`==` and `!=` compare the **values** of string objects, not references.

```csharp
string a == "hello";
string b == "h";
b += "ello";
// Equates to True
Console.WriteLine(a == b);
// Equates to False
Console.WriteLine(object.ReferenceEquals(a, b));
```

## Variables

Use implicit typing for local variables if type is obvious from right side of the assignment.

```csharp
var name = "John Smith";
var age = 42;
```
