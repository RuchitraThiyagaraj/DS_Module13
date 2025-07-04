# EX 1 Display operator precedence in the infix expression.
## DATE:
## AIM:
To write a C program to find and display the priority of the operator in the given Postfix expression

## Algorithm
1. Initialize a character array with an expression and loop through each character.
2. Check if the character is an operator (%, *, -, +, ^).
3. Call the priority() function to get the operator's priority level.
4. Use a switch statement to print the corresponding priority message.
5. End the program after processing all characters.

## Program:
```
/*
Program to find and display the priority of the operator in the given Postfix expression
Developed by: D VERGIN JENIFER
RegisterNumber: 212223240174
#include <stdio.h>
#include<string.h>

 /* Hint:
 int priority(char x)
{
  int result;
    if(x == '&' || x == '|')
        result=1;
        
        return result;
} Hint */

int main()
{
   int i,j;
   char ch[100]="K%L-M*N+(O^P)";
   for(i=0;i<strlen(ch);i++){
   if(ch[i]=='%'||ch[i]=='*'||ch[i]=='-'||ch[i]=='+'||ch[i]=='^'){
   j=priority(ch[i]);
       switch(j)
       {
           case 1:
           printf("%c  ----> Lowest Priority\n",ch[i]);
           break;
           case 2:
           printf("%c  ----> Second Lowest Priority\n",ch[i]);
           break;
           case 3:
           printf("%c  ----> Second Highest Priority\n",ch[i]);
           break;
           case 4:
           printf("%c  ----> Highest Priority\n",ch[i]);
           break;
    }
    }
    }return 0;
   
}
   
*/
```

## Output:

![pri](https://github.com/user-attachments/assets/08a8c9a9-483d-43eb-90e2-163c10ed5a40)

## Result:
Thus the C program to find and display the priority of the operator in the given Postfix expression is implemented successfully
