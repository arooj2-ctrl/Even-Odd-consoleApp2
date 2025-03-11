# EvenOdd Checker

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Requirements](#requirements)
- [Installation](#installation)
- [Usage](#usage)
- [Code Explanation](#code-explanation)
- [Comparison of Codes](#comparison-of-codes)
- [Contributing](#contributing)
- [License](#license)

## Introduction
This simple C# console application determines whether a given number is even or odd.

## Features
- Takes user input
- Determines if the number is even or odd
- Displays the result on the console

## Requirements
- .NET Framework or .NET Core
- C# Compiler

## Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/yourusername/EvenOddChecker.git
   ```
2. Navigate to the project directory:
   ```sh
   cd EvenOddChecker
   ```
3. Compile the program:
   ``` sh
   csc Program.cs
   ```

## Usage
1. Run the executable:
   ```sh
   ./Program.exe
   ```
2. Enter a number when prompted.
3. View the result indicating whether the number is even or odd.

## Code Explanation
The program prompts the user to enter a number, reads the input, and checks if it is divisible by 2.

```csharp
using System;

class EvenOdd
{
    static void Main()
    {
        int i;
        Console.WriteLine("Enter a number: ");
        i = int.Parse(Console.ReadLine());
        if (i % 2 == 0)
        {
            Console.WriteLine(i + " Is an Even Number");
            Console.ReadLine();
        }
        else
        {
            Console.WriteLine(i + " Is an Odd Number");
            Console.ReadLine();
        }
    }
}
```

## Comparison of Codes
The previous version of the code:
```csharp
using System;

class Program
{
    static void Main()
    {
        Console.Write("Enter a number: ");
        int number = Convert.ToInt32(Console.ReadLine());

        if (number % 2 == 0)
            Console.WriteLine($"{number} is an even number.");
        else
            Console.WriteLine($"{number} is an odd number.");
    }
}
```
### Key Differences:
1. **Class Name Change:** The class name was changed from `Program` to `EvenOdd` for better context.
2. **Variable Name Change:** The variable `number` was changed to `i`.
3. **Input Handling:** The new version uses `int.Parse()` instead of `Convert.ToInt32()`.
4. **Incorrect Syntax Fix:** The previous attempt to modify the code contained `if(i%2==o)` (using `o` instead of `0`), a syntax error that has been corrected.
5. **ReadLine() Usage:** The new version includes `Console.ReadLine();` after each output to keep the console open until user interaction.

## Contributing
Feel free to fork this repository and submit pull requests with improvements.

## License
This project is licensed under the MIT License.




