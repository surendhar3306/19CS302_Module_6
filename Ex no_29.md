# EX 29 C program to multiply two integer  numbers using pointers in which memory allocated using calloc(). 
## DATE:
## AIM:
To write a C program to multiply two integer  numbers using pointers in which memory allocated using calloc(). .

## Algorithm

1.Start the program and allocate memory for two integers using calloc().

2.Declare a variable s = 1 and a pointer res to store the result.

3.Read two integer values from the user using pointer notation.

4.Multiply the two values by accessing them through the pointer and store the result in s.

5.Display the result, free the allocated memory, and stop the program. 

## Program:
```
#include <stdio.h>
#include<stdlib.h>
int main()
{
  int s=1,*ptr;
  ptr = (int *)calloc(2,sizeof(int));
  int*res=&s;
  for(int i=0;i<2;i++)
  {
  
  scanf("%d",ptr+i);
  }
  
   for(int i=0;i<2;i++)
  {
  s=s*(*(ptr+i));
  }
  
  printf("The result is %d ",*res);
  free(ptr);
  return 0;
}
```

## Output:

<img width="438" height="256" alt="Screenshot 2026-03-19 155218" src="https://github.com/user-attachments/assets/64034991-d37b-4323-b6bd-0567c0b84b94" />


## Result:
Thus the program was executed and the output was verified successfully.
