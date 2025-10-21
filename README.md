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
#include <stdio.h>
int main() {
    int m,n;
    printf("Enter values of m and n:");
    scanf("%d %d",&m,&n);
    printf("Printing all Even values in the Range %d and %d :\n",m,n);
    while(m<=n){
        if(m%2==0){
            printf("%d ",m);
        }
        m++;
    }
    return 0;
}
```
## OUTPUT:
<img width="1455" height="480" alt="image" src="https://github.com/user-attachments/assets/cd307bbe-3f03-4ab9-94ec-a1ad4d244495" />










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
#include <stdio.h>
int main() {
    int row;
    printf("Enter Number of rows:");
    scanf("%d",&row);
    printf("Printing Triangle pattern\n");
    for(int i=1;i<=row;i++){
        for(int sp=1;sp<=row-i;sp++){
            printf(" ");
        }
        for(int j=1;j<=2*i-1;j++){
            if(i==row){
                printf("*");
            }
            else if(j==1 || j==2*i-1){
                printf("*");
            }
            else{
                printf(" ");
            }
        }
        printf("\n");
    }
    return 0;
}
```

## OUTPUT:

<img width="1435" height="782" alt="image" src="https://github.com/user-attachments/assets/75a0f41f-f697-4f4e-90cd-ef9cba737560" />




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
#include <stdio.h>
void add(int num1,int num2){
    printf("Result of Additon: %d",num1+num2);
}
void sub(int num1,int num2){
    printf("\nResult of Subtraction: %d",num1-num2);
}
int main() {
    int num1,num2;
    printf("two numbers to perform Addition and Subtraction:");
    scanf("%d %d",&num1,&num2);
    add(num1,num2);
    sub(num1,num2);
    return 0;
}
```

## OUTPUT:

<img width="1464" height="543" alt="image" src="https://github.com/user-attachments/assets/828a9fd8-94de-43a1-9580-d3ece2daa5f5" />





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
#include <stdio.h>
int main() {
    int num1,sum=0;
    printf("Enter a number:\n");
    scanf("%d",&num1);
    int temp=num1;
    while(temp>0){
        int rem=temp%10;
        if(rem%2!=0){
            sum+=rem;
        }
        temp/=10;
    }
    printf("Sum of all odd digits of %d is: %d",num1,sum);
    return 0;
}
```
## OUTPUT:

<img width="1440" height="549" alt="image" src="https://github.com/user-attachments/assets/db691a07-bf05-4c00-ace8-b58331921bdf" />



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
#include <stdio.h>
void fact(int i,int n){
    long a=1;
    for(int j=i;j<=n;j++){
        a*=j;
    }
    printf("Factorial of %d is %ld",n,a);
}
int main() {
    int num,i=1;
    printf("Enter number to find factorial for:");
    scanf("%d",&num);
    fact(i,num);
    return 0;
}
```

## OUTPUT:
<img width="1455" height="537" alt="image" src="https://github.com/user-attachments/assets/7a08039b-790b-4025-a5b8-8cac6b1d58d4" />

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
