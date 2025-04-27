# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <math.h> 

void calculateEMI(float principal, float rate, int months) {
    float emi;

    rate = rate / (12 * 100);

    emi = (principal * rate * pow(1 + rate, months)) / (pow(1 + rate, months) - 1);

    printf("The calculated EMI is: %.2f\n", emi);
}

int main() {
    float principal, rate;
    int months;

    printf("Enter the principal amount: ");
    scanf("%f", &principal);
    printf("Enter the annual interest rate (in percentage): ");
    scanf("%f", &rate);
    printf("Enter the number of months: ");
    scanf("%d", &months);

    calculateEMI(principal, rate, months);

    return 0;
}
```

## OUTPUT



![image](https://github.com/user-attachments/assets/1caa4cf7-83a0-408d-a462-9456a9605920)


## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n = 6; 
    int first = 0, second = 1, next;

    printf("Fibonacci series for %d terms:\n", n);

    for (int i = 1; i <= n; i++) {
        if (i == 1) {
            printf("%d ", first);
            continue;
        }
        if (i == 2) {
            printf("%d ", second);
            continue;
        }
        next = first + second; 
        first = second;        
        second = next;         
        printf("%d ", next);
    }

    printf("\n"); 
    return 0;
}

```
## OUTPUT



![image](https://github.com/user-attachments/assets/befc5850-618b-484f-a6b4-9fe2a4cbb449)





## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int array[n]; 

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    printf("The last element of the array is: %d\n", array[n - 1]);

    return 0;
}
```
## OUTPUT






![image](https://github.com/user-attachments/assets/ffd9d64b-be10-494e-b57a-1408684014c1)



## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n, count = 0;

    printf("Enter the number of elements: ");
    scanf("%d", &n);

    int array[n]; 

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);

        if (array[i] > 0) {
            count++; 
        }
    }

    printf("Total number of positive elements: %d\n", count);

    return 0;
}

```

## OUTPUT



![image](https://github.com/user-attachments/assets/8276c2cb-5c23-44dc-803c-4453d817b6b4)


## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```c
#include <stdio.h>

int main() {
    int n;

    printf("Enter the number of elements in the array: ");
    scanf("%d", &n);

    int array[n]; 
    char updatedArray[n]; 

    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &array[i]);
    }

    for (int i = 0; i < n; i++) {
        if (array[i] % 2 == 0) {
            updatedArray[i] = 'E'; 
        } else {
            updatedArray[i] = array[i]; 
        }
    }

    printf("Updated array:\n");
    for (int i = 0; i < n; i++) {
        if (updatedArray[i] == 'E') {
            printf("%c ", updatedArray[i]); 
        } else {
            printf("%d ", updatedArray[i]); 
        }
    }

    printf("\n"); 
    return 0;
}
```
## Output:
 
![image](https://github.com/user-attachments/assets/75fb20b4-e277-453c-8998-acc2bc9814da)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



