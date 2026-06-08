# # Pointers: Vowel or Consonant Checker Using Pointers in C

## 🎯 Aim

To write a C program to determine whether a character is a vowel or a consonant using a pointer.

## 🧠 Algorithm

1. **Input**:
   - Read a character from the user.
   - Store the character's address in a pointer variable `pch`.

2. **Check Vowel**:
   - Use an `if` or `switch` statement to check if the character pointed to by `pch` is one of the vowels: `'A'`, `'E'`, `'I'`, `'O'`, `'U'` (uppercase only).
   - If it matches any of these, it is a **vowel**.
   - Otherwise, it is a **consonant**.

3. **Output**:
   - Print whether the input character is a vowel or consonant.

## Program
```
#include <stdio.h>
int main() {
    char ch;
    char *pch = &ch;  
    printf("Enter an uppercase alphabet: ");
    scanf(" %c", pch);  // Notice the space before %c to consume any leftover newline
    if (*pch == 'A' || *pch == 'E' || *pch == 'I' || *pch == 'O' || *pch == 'U') {
        printf("The character %c is a vowel.\n", *pch);
    } else {
        printf("The character %c is a consonant.\n", *pch);
    }
    return 0;
}
```

## Output
```
Enter an uppercase alphabet: E
The character E is a vowel.
Enter an uppercase alphabet: G
The character G is a consonant.
```




## Result
The above programme is implemented and executed.
