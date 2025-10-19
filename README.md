# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int m,n;
    printf("Enter the value for M and N\n");
    scanf("%d %d",&m,&n);
    for (int i=m;i<=n;i++)
    {
        if (i%2 == 0)
        {
            printf("%d ",i);
        }
    }
}
```

## OUTPUT:

![alt text](<Screenshot (14).png>)

## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int row;
    scanf("%d",&row);
    for (int i=1;i<=row;i++)
    {
        for (int col=1;col<=i;col++)
        {
            printf("* ");
        }
        printf("\n");
    }
}

```


## OUTPUT:

![alt text](<Screenshot 2025-10-19 093140.png>)



## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
```
#include<stdio.h>
void add(int a,int b)
{
    printf("Addition of %d and %d is %d\n",a,b,a+b);
}
void sub(int a,int b)
{
    printf("Subtraction of %d and %d is %d",a,b,a-b);
}
int main()
{
    int x,y;
    scanf("%d %d",&x,&y);
    add(x,y);
    sub(x,y);

}
```


## OUTPUT:


![alt text](<Screenshot 2025-10-19 093018.png>)



## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
```
#include<stdio.h>
int main()
{
    int sum=0;
    int h;
    scanf("%d",&h);
    for(int i=h;i!=0;i/=10)
    {
        int v=i%10;
        if (v%2 == 1)
        {
            sum+=v;
        }
    }
    printf("The sum of odd digits in the given number is %d",sum);
}
```

## OUTPUT:

![alt text](<Screenshot 2025-10-19 092830.png>)


## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
```
#include<stdio.h>
void fact()
{
    int n;
    scanf("%d",&n);
    int i=1,fact=1;
    while(i<=n)
    {
        fact=fact*i;
        i++;
    }
    printf("The factorial of the number %d is %d",n,fact);
}
int main()
{
   fact();
}
```


## OUTPUT:

![alt text](<Screenshot (15).png>)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
