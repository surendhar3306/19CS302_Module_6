# EX 30 C program to add three integer elements in an array using realloc() and that array already has four elements.
## DATE:
## AIM:
To write a C program to add three integer elements in an array using realloc() and that array already has four elements.

## Algorithm

1.Start the program and allocate memory for an array of 4 integers using malloc().

2.Initialize the first four elements of the array.

3.Use realloc() to resize the array to hold 7 elements.

4.Add three more integer elements to the resized array.

5.Display all the elements of the array and stop the program.

## Program:
```
#include<stdio.h>
#include<stdlib.h>
int main()
{
    int *p,*np;
    p=(int*)malloc(7*sizeof(int));
    p[0]=1;
    p[1]=2;
    p[2]=3;
    p[3]=4;
    
    np=(int*)realloc(p,sizeof(int));
    np[4]=12;
    np[5]=10;
    np[6]=8;
    
    for(int i=0;i<7;i++)
    {
        printf("%d ",np[i]);
    }
    
}
```

## Output:

<img width="372" height="125" alt="Screenshot 2026-03-19 154922" src="https://github.com/user-attachments/assets/d6cccd52-adcb-4f6e-8c12-d8075f6dfc05" />


## Result:
Thus the program was executed and the output was verified successfully.
