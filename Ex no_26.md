# EX 26 C program to calculate the total and average of student using structure.
## DATE:
## AIM:
To write a C program to calculate the total and average of student using structure.
## Algorithm

1.Start the program and define a structure student with fields for name, roll number, subjects, and total.

2.Read the number of students n and declare an array of structures.

3.For each student, read marks of 5 subjects and calculate the total by summing them.

4.Compute the average for each student using average = total / 5.

5.Display the total and average for each student and stop the program.

## Program:
```
#include <stdio.h>
struct student {
    char name[10];
    int rollno;
    int subject[5];
    int total;
};

int main() {
    int n, i, j;

    scanf("%d", &n);
    
    struct student s[n];
    for(i = 0; i < n; i++) {
        s[i].total = 0;
        for(j = 0; j < 5; j++)
        {
            scanf("%d", &s[i].subject[j]);
            s[i].total += s[i].subject[j];
        }
    }

    
    for(i = 0; i < n; i++) {
        printf("%d\n", s[i].total);
    }

    return 0;
}

```

## Output:

<img width="365" height="175" alt="Screenshot 2026-03-19 163601" src="https://github.com/user-attachments/assets/3623c00d-790a-4663-89f2-1cd9c70adfd6" />


## Result:
Thus the program was executed and the output was verified successfully.
