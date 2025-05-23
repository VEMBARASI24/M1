
# EX-01-Datatypes-Operators
## NAME:Vembarasi.A.R
## REGISTER NUMBER:212224220120
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
```
 #include <stdio.h>
int main()
{
    char ch,ch1,ch2;
    scanf("%c%c%c",&ch,&ch1,&ch2);
    printf("The reverse of %c%c%c is %c%c%c",ch,ch1,ch2,ch2,ch1,ch);
    return 0;
    
}
```

## OUTPUT:
![Screenshot 2025-04-28 132917](https://github.com/user-attachments/assets/f5879790-ae6f-490f-b30b-169c16f3091c)

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
```
#include <stdio.h>
int main()
{
    int a;
    scanf("%d",&a);
    if (a>=0)
    {
        printf("Number is positive.");
    }
    else
    {
        printf("Number is negative.");
    }
    return 0;
}
```

# OUTPUT:
![image](https://github.com/user-attachments/assets/bbe17dd9-092a-4151-b17d-7585b6334f0c)

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
```
#include <stdio.h>
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if (a<b)
    {
        printf("Minimum between %d and %d is %d",a,b,a);
    }
    else
    {
        printf("Minimum between %d and %d is %d",a,b,b);
    }
    return 0;
}
```

## OUTPUT:

![Screenshot 2025-04-28 133203](https://github.com/user-attachments/assets/69a60332-728a-447b-9af4-ce6b7e61d800)

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
```
#include <stdio.h>
int main(){
    int a;
    scanf("%d",&a);
    if(a==1)
       printf("TRUE");
       
   
}
```

## OUTPUT:

![Screenshot 2025-04-28 133309](https://github.com/user-attachments/assets/76a3b3b3-cb13-476f-bbe7-d4c3b94b6ed1)

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
```
#include <stdio.h>

int main() {
    int marks1, marks2, marks3;
    int total;
    float percentage;
    int min_marks = 35;
    printf("Enter marks for subject 1: ");
    scanf("%d", &marks1);

    printf("Enter marks for subject 2: ");
    scanf("%d", &marks2);

    printf("Enter marks for subject 3: ");
    scanf("%d", &marks3);

    if (marks1 < min_marks || marks2 < min_marks || marks3 < min_marks) {
        printf("Result: Fail (One or more subjects below minimum marks)\n");
        return 0;
    }

    total = marks1 + marks2 + marks3;
    percentage = (total / 300.0) * 100;

    printf("Total marks = %d\n", total);
    printf("Percentage = %.2f%%\n", percentage);

    if (percentage >= 60) {
        printf("Division = First\n");
    } else if (percentage >= 50) {
        printf("Division = Second\n");
    } else if (percentage >= 35) {
        printf("Division = Pass\n");
    } else {
        printf("Result = Fail\n");
    }

    return 0;
}


```
## OUTPUT:

![Screenshot 2025-04-28 133412](https://github.com/user-attachments/assets/4cdd406f-2ea9-4941-80f2-9b77f0142483)


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

