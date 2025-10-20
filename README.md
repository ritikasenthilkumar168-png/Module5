# NAME: Ritika. S
# REGISTER NO: 25009202

# EXPNO: 5a) C PROGRAM TO TEST WHETHER THE NUMBER IS EQUAL TO ZERO OR NOT BY USING POINTERS.

# AIM:
To write a C program to test whether the number is equal to zero or not by using pointers. 

# ALGORITHM:
1. Take the number from the user as input using scanf function.
2. Assign the address of the number into the integer pointer.
3. Using nested if statements, check whether the number is equal to zero, positive or negative.
4. Print the statements given in the blocks using printf function.

# PROGRAM:

```
#include<stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    int *ptr=&num;
    if(*ptr==0) printf("the number is equal to zero");
    else if(*ptr>0) printf("the number is Positive");
    else printf("the number is Negative");
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 150345.png>)

# RESULT:
Thus, the program is verified successfully.


# EXPNO: 5b) C PROGRAM TO CALCULATE THE POWER FOR 8,4 USING RECUSRION.

# AIM:
To write a C program to calculate the power for 8,4 using recursion.

# ALGORITHM:
1. Declare a function with arguments with return types.
2. Inside that function, set the base case.
3. Inside main() function, declare the base nad exponent values.
4. Call the function and then print the value using printf function.

# PROGRAM:

```
#include<stdio.h>
int power(int base, int exponent)
{
    if(exponent==0) return 1;
    else return base*power(base,exponent-1);
}
int main()
{
    int base=8,exponent=4;
    printf("%d^%d = %d",base,exponent,power(base,exponent));
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 150951.png>)

# RESULT:
Thus, the program is verified successfully.


# EXPNO: 5c) C PROGRAM TO FIND SUM OF EACH ROW OF A MATRIX.
```
INPUT

PLEASE ENTER NUMBER OF ROWS AND COLUMNS : 3 3
INPUT ELEMENTS OF MATRIX:
1 2 3
4 5 6
7 8 9
```

# AIM:
To write a C Program to find Sum of each row of a Matrix.
```
Input

Please Enter Number of rows and columns  : 3 3
Input elements of matrix:
1 2 3
4 5 6
7 8 9
```

# ALGORITHM:
1. Inside main() function, declare rows and cols and then take them from the user using scanf function.
2. Declare an integer matrix.
3. Using for loops, take the matrix from the user as input using scanf function.
4. Then, do the calcultaion to find the sum.
5. Print the sum using printf function.

# PROGRAM:

```
#include <stdio.h>
int main()
{
    int rows,cols;
    scanf("%d %d",&rows,&cols);
    int matrix[rows][cols];
    for(int i=0;i<rows;i++)
    {
        for(int j=0;j<cols;j++)
        {
            scanf("%d",&matrix[i][j]);
        }
    }
    for(int i=0;i<rows;i++)
    {
        int rowSum=0;
        for(int j=0;j<cols;j++)
        {
            rowSum+=matrix[i][j];
        }
        printf("The Sum of Elements of a Rows in a Matrix:  %d\n",rowSum);
    }
    return 0;
}

```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 151825.png>)

# RESULT:
Thus, the program is verified successfully.


# EXPNO: 5d) C PROGRAM TO WRITE A PROGRAM TO COUNT TOTAL NUMBER OF ALPHABETS IN A STRING USING BUILT-IN FUNCTIONS.

# AIM:
To write a program in C to count total number of alphabets in a string using built-in functions. 

# ALGORITHM:
1. Use the header file #include<ctype.h>.
2. Inside main() function, declare a string and using fgets() function, take the string as an input from the user.
3. Using for loop, do the iteration to count the number of alphabets.
4. Print the count using printf function.

# PROGRAM:

```
#include<stdio.h>
#include<ctype.h>
int main()
{
    char str[100];
    int count=0;
    fgets(str,sizeof(str),stdin);
    for(int i=0;str[i]!='\0';i++)
    {
        if(isalpha(str[i]))
        {
            count++;
        }
    }
    printf("Number of Alphabets in the string is : %d\n",count);
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 152501.png>)

# RESULT:
Thus, the program is verified successfully.


# EXPNO: 5e) C PROGRAM TO WRITE A PROGRAM TO CHECK WHETHER THE NUMBER 500 IS EVEN NUMBER OR ODD NUMBER USING POINTERS.

# AIM:
To write a C program to check whether the number 500 is even number or odd number using pointers.  

# ALGORITHM:
1. Take the number from the user as input using scanf function.
2. Assign the address of the number into the integer pointer.
3. Using if condition, check whether the number is even or odd.
4. If the condition is not true, then the else block will be executed.

# PROGRAM:

```
#include<stdio.h>
int main()
{
    int num;
    scanf("%d",&num);
    int* ptr=&num;
    if(*ptr%2==0) printf("%d is even.",num);
    else printf("%d is odd.",num);
    return 0;
}
```

# OUTPUT:
![alt text](<Screenshot 2025-10-20 153021.png>)

# RESULT:
Thus, the program is verified successfully.


