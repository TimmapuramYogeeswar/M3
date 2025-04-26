## NAME-TIMMAPURAM YOGEESWAR  
## DATE-26-04-2025
## EX-11-EMI-CALCULATOR

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
```
#include <stdio.h>
#include <math.h>
void calculateEMI(float principal, float annualRate, int tenureYears);

int main() {
    float principal, annualRate;
    int tenureYears;
    printf("Enter loan amount (principal): ");
    scanf("%f", &principal);
    printf("Enter annual interest rate (in %%): ");
    scanf("%f", &annualRate);
    printf("Enter loan tenure (in years): ");
    scanf("%d", &tenureYears);
    calculateEMI(principal, annualRate, tenureYears);
    return 0;
}
void calculateEMI(float principal, float annualRate, int tenureYears) {
    float monthlyRate = annualRate / (12 * 100); 
    int tenureMonths = tenureYears * 12;
    float emi;

    emi = (principal * monthlyRate * pow(1 + monthlyRate, tenureMonths)) /
          (pow(1 + monthlyRate, tenureMonths) - 1);

    printf("\nYour EMI is: ₹%.2f per month\n", emi);
}

```

## OUTPUT

![Screenshot 2025-04-26 173841](https://github.com/user-attachments/assets/98f1ff1a-c32c-427c-9ece-ea2bda9dde3a)

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
```
#include <stdio.h>
int main() {
    int n = 6;  
    int first = 0, second = 1, next;
    printf("Fibonacci series for %d terms:\n", n);
    for (int i = 0; i < n; i++) {
        if (i <= 1)
            next = i;
        else {
            next = first + second;
            first = second;
            second = next;
        }
        printf("%d ", next);
    }
    printf("\n");
    return 0;
}

```
## OUTPUT

![Screenshot 2025-04-26 173947](https://github.com/user-attachments/assets/70ba65b5-73c7-4099-8858-03971ee73aa5)

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
```
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("The last element is: %d\n", arr[n - 1]);

    return 0;
}

```
## OUTPUT

![Screenshot 2025-04-26 174155](https://github.com/user-attachments/assets/2ba03c93-4451-47f4-8525-6629ec9cc79c)

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
```
#include <stdio.h>
int main() {
    int n, count = 0;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d elements:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }
    printf("Total number of positive elements = %d\n", count);

    return 0;
}

```
## OUTPUT

![Screenshot 2025-04-26 174318](https://github.com/user-attachments/assets/6b8459f3-24fd-4afc-a535-b84b0f575f42)

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
```
#include <stdio.h>
int main() {
    int n;
    printf("Enter the number of elements: ");
    scanf("%d", &n);
    int arr[n];
    printf("Enter %d integers:\n", n);
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("Modified array (even elements replaced with 'E'):\n");
    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");
    return 0;
}

```
## Output:

![Screenshot 2025-04-26 174746](https://github.com/user-attachments/assets/21e133aa-f4a2-4ddf-aa7a-e2acfad6ad07)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



