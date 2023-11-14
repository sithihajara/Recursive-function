# Recursive-function

## Aim:
To write a C# program to reverse a number using recursive function.

## Algorithm:
### Step 1:
Create a function for reversing.

### Step 2:
Get the number from the user.

### Step 3:
In the function find reminder of the number and multiply it by 10 and add the reverse number.

### Step 4:
Recusively call this function to get the reversed number.

### Step 5:
print the reversed number.
## Program:
```
Developed by: Sithi Hajara I
Register Number: 212221230102
```
```
using System;
namespace Recursive_Function
{
    class Program
    {
        public static int m, reverse = 0;
        public static int Recur(int number)
        {
            
            if (number > 0)
            {
                Program.m = number % 10;
                Program.reverse = Program.reverse * 10 + m;
                number = number / 10;
                return Recur(number);
            }
            return Program.reverse;

        }
        static void Main(string[] args)
        {
            int num;
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine(Recur(num));
        }
    }
}
```
## Output:
![238124759-d11d3f6f-4927-47d4-b1a6-d2babf07f6f4](https://github.com/MEENA155/Recursive-function/assets/94677128/03f7bac2-41d9-4899-9369-0bd935b49ab3)

## Result:
Thus the C# program to reverse a number using recursive function is executed successfully.
