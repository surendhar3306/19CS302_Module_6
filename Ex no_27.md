# EX 27 Create a C program to read and display 3 book details using array of structures.
## DATE:
## AIM:

To write a C program to read and display 3 book details using array of structures.

## Algorithm

1.Start the program and define a structure book with fields title, author, publication, and price.

2.Declare an array of structures to store details of 3 books.

3.Use a loop to read the details (title, author, publication, price) for each book.

4.Use another loop to access and display the stored book details.

5.Stop the program.

## Program:
```
#include<stdio.h>
struct book{
    char title[100];
    char author[50];
    char publication[100];
    float price;
};
int main()
{
    struct book books[3];
    for(int i=0;i<3;i++)
    {
        
        scanf(" %[^\n]",books[i].title);
        scanf(" %[^\n]",books[i].author);
        scanf(" %[^\n]",books[i].publication);
        scanf("%f",&books[i].price);
    }
    for(int i=0;i<3;i++)
    {
        printf("Title: %s\n",books[i].title);
        printf("Author: %s\n",books[i].author);
        printf("Publication: %s\n",books[i].publication);
        printf("Price: %.2f",books[i].price);
    }
}
```

## Output:

<img width="638" height="360" alt="Screenshot 2026-03-19 163113" src="https://github.com/user-attachments/assets/680ca262-dbd1-4d67-a857-252b97679156" />


## Result:
Thus the program was executed and the output was verified successfully.
