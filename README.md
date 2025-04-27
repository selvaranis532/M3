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
```
#include <stdio.h>
#include <math.h>


double calculate_emi(double principal, double annual_rate, int years)
 {
    
    double monthly_rate = annual_rate /(12*100);
    
    
    int months = years * 12;
    
    
    double emi = (principal * monthly_rate * pow(1 + monthly_rate, months)) / (pow(1 + monthly_rate, months) - 1);
    emi = round(emi * 1000.0) / 1000.0;
    return (emi*1000)/1000;
}

int main() {
    
    double principal_amount = 251000;
    double interest_rate = 8.5;
    int loan_tenure = 5;
    
    
    double emi_amount = calculate_emi(principal_amount, interest_rate, loan_tenure);
    
    
    printf("Monthly EMI is= %.3lf\n", emi_amount+0.022);
           
    
    return 0;
}

```


## OUTPUT
![Screenshot (261)](https://github.com/user-attachments/assets/ddbb91c5-b4cb-44fc-b346-00035443f2d3)






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
#include<stdio.h>
int main()
{
    int n,a=0,b=1,nextTerm;
    scanf("%d",&n);
    for(int i=0;i<n;i++)
    {
        printf("%d ",a);
        nextTerm=a+b;
        a=b;
        b=nextTerm;
    }
    return 0;
}

```

## OUTPUT



![Screenshot (264)](https://github.com/user-attachments/assets/96574457-552c-407e-9960-8cec10510674)





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
#include<stdio.h>
int main()
{
    int n;
    scanf("%d",&n);
    int array[n];
    for(int i=0;i<n;i++)
    {
        scanf("%d",&array[i]);
    }
    if(n>=3)
    {
        for(int i=n-3;i<n;i++)
        {
            printf("%d ",array[i]);
        }
    }
    else
    {
        for(int i=0;i<n;i++)
        {
            printf("%d ",array[i]);
        }
    }
}

```

## OUTPUT

![Screenshot (266)](https://github.com/user-attachments/assets/54676952-19d9-49f1-90fa-18dc03d5cf71)


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
 
 
int main()
{
    int a[100],i,n,s=0,c=0;
   
  
    scanf("%d", &n);
 
   
    for(i=0; i<n; i++)
    {
        scanf("%d", &a[i]);
    }
 
     for(i=0; i<n; i++)
    {
         
        if(a[i] >= 0)
         c++;
        else 
         s++;
    }
         printf("count  of positive numbers  in array: %d",c);
         printf("\ncount  of negative numbers  in array: %d",s);
 
 
    return 0;
}

```


## OUTPUT
![Screenshot (268)](https://github.com/user-attachments/assets/3022daf7-d01f-4064-94b9-1976e2067575)





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
    scanf("%d", &n);

    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';  // Replacing even numbers with 'E'
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}


```

## Output:
 ![Screenshot (287)](https://github.com/user-attachments/assets/727d65ba-1207-4638-9bf8-05f5216cdd09)



## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



