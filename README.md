Here’s your **README.md** file with a **Table of Contents** for better navigation:

---

# **Even Odd Program in C#**

## Table of Contents  
- [Description](#description)  
- [Installation](#installation)  
- [Usage](#usage)  
- [Example Output](#example-output)  
- [Code](#code)  
- [License](#license)  

---

## **1. Description**  
This is a simple C# console application that determines whether a given number is even or odd.  

- The program takes an integer input from the user.  
- It checks if the number is divisible by 2 using the modulus (`%`) operator.  
- If the remainder is `0`, it prints that the number is even; otherwise, it prints that the number is odd.  

## **2. Installation**  
To run this program, follow these steps:  

1. Install [Visual Studio](https://visualstudio.microsoft.com/) or any C#-compatible editor.  
2. Clone this repository using Git:  
   ```sh
   git clone https://github.com/your-username/your-repo-name.git
   ```
3. Open the project in Visual Studio or any C# editor.  
4. Compile and run the program.  

## **3. Usage**  
1. Run the program.  
2. Enter an integer when prompted.  
3. The program will analyze the number and display whether it is even or odd.  

## **4. Example Output**  

### **Case 1: When the user enters `5`**  
```sh
Enter a number: 5
5 is an odd number.
```
### **Case 2: When the user enters `8`**  
```sh
Enter a number: 8
8 is an even number.
```

## **5. Code**  
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

## **6. License**  
This project is open-source and available under the [MIT License](LICENSE).  

---

###  **How the Table of Contents Works:**  
The `(#section-name)` links allow users to jump to different sections within the README when viewed on GitHub.

