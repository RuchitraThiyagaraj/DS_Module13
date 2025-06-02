# EX3 Implementation of Tower of Hanoi
## DATE:
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. If number of disks `n` > 0, recursively move `n-1` disks from source to auxiliary.
2. Print the move of the nth disk from source to destination.
3. Recursively move `n-1` disks from auxiliary to destination.
4. Repeat steps until all disks are moved from source to destination following the rules.
5. Start the process by calling TOH(n, source, destination, auxiliary) in `main`.  

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: T.RUCHITRA
RegisterNumber: 21222311043
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
    if(n>0)
    {
    TOH(n-1,x,z,y);
    printf("%c to %c",x,y);
    printf("\n");
    TOH(n-1,z,y,x);
    }
    
}
int main()
{
    int n=3;
    TOH(n,'A','B','C');
}
*/
```

## Output:

![Output](img/toh.png)

## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
