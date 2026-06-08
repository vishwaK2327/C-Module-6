## Structures: Student Information Storage (C Program)
## Aim
Create a C program to store and display the information of 5 students using an array of structures.

## Algorithm
1. Input: Read the name and marks of 5 students into an array of structures s.

2. Display Information:

    Iterate through the array and print the roll number, name, and marks for each student.

3.End the program execution.

## Program
```
#include <stdio.h>
struct Student {
    char name[50];
    float marks;
};
int main() {
    struct Student s[5]; 
    int i;
    printf("Enter the name and marks of 5 students:\n");
    for (i = 0; i < 5; i++) {
        printf("\nStudent %d\n", i + 1);
        printf("Name: ");
        scanf(" %[^\n]", s[i].name); 
        printf("Marks: ");
        scanf("%f", &s[i].marks);
    }
    printf("\nStudent Information:\n");
    printf("Roll No\tName\t\tMarks\n");
    for (i = 0; i < 5; i++) {
        printf("%d\t%-15s %.2f\n", i + 1, s[i].name, s[i].marks);
    }
    return 0;
}
```

## Output
```
Enter the name and marks of 5 students:

Student 1
Name: Alice
Marks: 89.5

Student 2
Name: Bob
Marks: 76

Student 3
Name: Charlie
Marks: 91.25

Student 4
Name: Diana
Marks: 85

Student 5
Name: Ethan
Marks: 78.75

Student Information:
Roll No Name            Marks
1       Alice           89.50
2       Bob             76.00
3       Charlie         91.25
4       Diana           85.00
5       Ethan           78.75
```


## Result
The above programme is implemented and executed.

