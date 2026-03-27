# EX 28 C program to print the values of the weekdays based on the following enum declaration.
enum day {sunday = 1, monday, tuesday = 5,wednesday, thursday = 10, friday, saturday};

## DATE:
## AIM:
To write a C program to print the values of the weekdays based on the following enum declaration.
enum day {sunday = 1, monday, tuesday = 5,wednesday, thursday = 10, friday, saturday};

## Algorithm

1.Start the program and declare an enumeration day with assigned values for weekdays.

2.Define the enum constants with specific and default values as given.

3.In the main() function, access each enum constant.

4.Print the values of all the weekdays using printf().

5.Stop the program.

## Program:
```
#include <stdio.h>

enum day {
    sunday = 1,
    monday,
    tuesday = 5,
    wednesday,
    thursday = 10,
    friday,
    saturday
};

int main() {
    printf("%d %d %d %d %d %d %d\n", 
        sunday,     
        monday,     
        tuesday,    
        wednesday,  
        thursday,   
        friday,     
        saturday   
    );

    return 0;
}

```

## Output:

<img width="346" height="120" alt="Screenshot 2026-03-19 155751" src="https://github.com/user-attachments/assets/a63b93e5-4323-42c1-af3c-77fabe1ef22d" />



## Result:
Thus the program was executed and the output was verified successfully.
