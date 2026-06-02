# EX 9 C program to find the sum of odd digits using do while loop.
## DATE:
## AIM:
To write a C program to find the sum of odd digits using do while loop.

## Algorithm
1. Start.
2. Read num.
3. Convert num to positive if negative.
4. Initialize sum = 0
5. do-while loop:
6. Get last digit
7. If odd, add to sum
8. Remove last digit
9. Repeat until num == 0
10. Print sum
11. End.
    
## Program:
```
#include <stdio.h>
int main() {
    int num, digit, sum = 0;
    scanf("%d", &num);
    if (num < 0) {
        num = -num;
    }
    do {
        digit = num % 10;
        if (digit % 2 != 0) { 
            sum += digit;
        }
        num = num / 10;
    } while (num != 0);
    printf("Sum of odd digits is: %d\n", sum);
    return 0;
}
```

## Output:
<img width="263" height="55" alt="image" src="https://github.com/user-attachments/assets/538cdf7f-bfbe-429d-8e10-8e3507a6f357" />


## Result:
Thus the program was executed and the output was verified successfully.
