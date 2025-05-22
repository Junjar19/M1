
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
``` c
#include <stdio.h>

int main() 
{
    char char1, char2, char3;

    printf("Enter the first character: ");
    scanf(" %c", &char1);
    printf("Enter the second character: ");
    scanf(" %c", &char2);
    printf("Enter the third character: ");
    scanf(" %c", &char3);

    printf("Characters in reverse order: %c %c %c\n", char3, char2, char1);

    return 0;
}
```
## OUTPUT:

![image](https://github.com/user-attachments/assets/6c719f22-23ed-4c0c-bba4-0a171428988b)











## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
``` c
#include <stdio.h>

int main() {
    int A;

    printf("Enter a value for A: ");
    scanf("%d", &A);

    if (A > 0) {
        printf("A is a positive number.\n");
    } else {
        printf("A is not a positive number.\n");
    }

    return 0;
}

```
# OUTPUT:
![image](https://github.com/user-attachments/assets/1493dc21-bb1c-4c03-b4a0-6300a2229b50)










# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
``` c
#include <stdio.h>

int main() {
    int num1, den1, num2, den2;
    float fraction1, fraction2, min;

    printf("Enter the numerator and denominator of the first fraction: ");
    scanf("%d %d", &num1, &den1);

    printf("Enter the numerator and denominator of the second fraction: ");
    scanf("%d %d", &num2, &den2);

    fraction1 = (float)num1 / den1;
    fraction2 = (float)num2 / den2;

    min = (fraction1 < fraction2) ? fraction1 : fraction2;

    printf("The smaller fraction in decimal form is: %.2f\n", min);

    return 0;
}

```
## OUTPUT:

![image](https://github.com/user-attachments/assets/035d1f40-4fbc-48ed-b551-272339e9d03b)







## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
``` c
#include <stdio.h>

int main() {
    int input;

    printf("Enter a value: ");
    scanf("%d", &input);

    if (input == 1) {
        printf("The input value is equal to 1.\n");
    } else {
        printf("The input value is not equal to 1.\n");
    }

    return 0;
}

```
## OUTPUT:

### Value not equals to 1
![image](https://github.com/user-attachments/assets/005cbe49-00fb-451c-93cf-6252c2ecfecf)

### Value equals to 1
![image](https://github.com/user-attachments/assets/ed940a6d-7612-4ed0-b81b-de0771fab6dd)







	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:
``` c
#include <stdio.h>

int main() {
    int m1, m2, m3; 
    float tot, per; 

    printf("Enter marks for Subject 1: ");
    scanf("%d", &m1);
    printf("Enter marks for Subject 2: ");
    scanf("%d", &m2);
    printf("Enter marks for Subject 3: ");
    scanf("%d", &m3);

    tot = m1 + m2 + m3;
    per = tot / 3.0;

    printf("Total Marks = %.2f\n", tot);
    printf("Percentage = %.2f\n", per);

    if (m1 >= 40 && m2 >= 40 && m3 >= 40) {
        if (per >= 60) {
            printf("Division = First\n");
        } else if (per >= 48) {
            printf("Division = Second\n");
        } else if (per >= 36) {
            printf("Division = Pass\n");
        } else {
            printf("Division = Fail\n");
        }
    } else {
        printf("Division = Fail\n");
    }

    return 0;
}

```
## OUTPUT:
![image](https://github.com/user-attachments/assets/3dfce193-d1de-4405-9b6f-ff88cb778a24)
## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

