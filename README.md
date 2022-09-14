# Pattern

## Aim:
To write a C# program to print the pascal triangle

## Algorithm:
step1:
Start

step2:
Declare variables rows,val,i,j,blank

step3:
Initialize the value of variables, i=0,j=0,val=1

step4:
Enter the limit

step5:
using for loop printing " " when i&j==0 and using for loop applying the concept of pascal triangle

## Program:
~~~
using System;
namespace PascalTriangleDemo
{
    class Example
    {
        public static void Main()
        {
            int rows = 5, val = 1, blank, i, j;
            for (i = 0; i < rows; i++)
            {
                for (blank = 1; blank <= rows - i; blank++)
                    Console.Write(" ");
                for (j = 0; j <= i; j++)
                {
                    if (j == 0 || i == 0)
                        val = 1;
                    else
                        val = val * (i - j + 1) / j;
                    Console.Write(val + " ");
                }
                Console.WriteLine();
            }
        }
    }
}
~~~

## Output:
![image](https://user-images.githubusercontent.com/94187572/190058042-9ebe1516-d8f7-4b7a-8d78-d8bdf68cd28f.png)


## Result:
Thus the C# program to display pascal triangle is exucuted sucessfully.


