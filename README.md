# Digit Power Sum - Recursive Calculation

## Description

This assignment requires you to write a C# program that calculates the sum of the cubes of the digits of a given integer using recursion.

## Instructions

1.  **Clone the Repository:** Clone this repository to your local machine.
2.  **Implement the `CalculateDigitPowerSum` Function:** Open the `DigitPowerSum.cs` file and implement the `CalculateDigitPowerSum` function. This function should:
    * Take an integer `n` as input.
    * Separate each digit of the input number.
    * Calculate the cube (power of 3) of each digit.
    * Use recursion to calculate the sum of the cubed digits.
    * Return the final sum.
3.  **Input Validation:** Your program should handle invalid input. Specifically, if the input number is not greater than 2000, it should display an error message.
4.  **Testing:** Test your implementation with the provided test cases (see below) and any additional test cases you create.
5.  **Commit and Push:** Commit your changes and push them back to your GitHub repository.
6.  **Submission:** Your code will be automatically submitted through GitHub Classroom.

Test Cases

Input: 3142
Expected Output: 100 (3^3 + 1^3 + 4^3 + 2^3 = 27 + 1 + 64 + 8 = 100)

Input: 2001
Expected Output: 9 (2^3 + 0^3 + 0^3 + 1^3 = 8 + 0 + 0 + 1 = 9)

Input: 5231
Expected Output: 161 (5^3 + 2^3 + 3^3 + 1^3 = 125 + 8 + 27 + 1 = 161)

Input: 9999
Expected Output: 2916 (9^3 + 9^3 + 9^3 + 9^3 = 729 + 729 + 729 + 729 = 2916)

Input: 4321
Expected Output: 100 (4^3 + 3^3 + 2^3 + 1^3 = 64 + 27 + 8 + 1 = 100)

Input: 2500
Expected Output: 133 (2^3 + 5^3 + 0^3 + 0^3 = 8 + 125 + 0 + 0 = 133)

## Starter Code (DigitPowerSum.cs)

```csharp
using System;

public class DigitPowerSum
{
    public static int CalculateDigitPowerSum(int n)
    {
        // Your recursive code here
        return 0; // Placeholder
    }

    public static void Main(string[] args)
    {
        Console.WriteLine("Enter a number greater than 2000:");
        if (int.TryParse(Console.ReadLine(), out int input) && input > 2000)
        {
            int result = CalculateDigitPowerSum(input);
            Console.WriteLine("Result: " + result);
        }
        else
        {
            Console.WriteLine("Invalid input. Please enter a number greater than 2000.");
        }
    }
}


