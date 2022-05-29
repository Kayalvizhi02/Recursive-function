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
```c#

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
            Console.WriteLine("Enter a Number to reverse: ");
            num = Convert.ToInt32(Console.ReadLine());
            Console.WriteLine("Reversed Number is " + Recur(num));

        }
    }
    
}

```
## Output:

![img](https://user-images.githubusercontent.com/75413726/170868793-b6ea0da8-8f84-4233-a6c0-e75d5f507edb.jpg)


## Result:

Thus the C# program to reverse a number using recursive function is executed successfully.


