# C-Day-56-Count-Positive-Negative-Zero
# C Day 56 - Count Positive, Negative and Zero

This program takes multiple numbers from the user and counts how many numbers are positive, negative, and zero.

## Example Input

```text
Enter how many numbers: 6
Enter number 1: 10
Enter number 2: -5
Enter number 3: 0
Enter number 4: 20
Enter number 5: -8
Enter number 6: 15
```

## Output

```text
Positive numbers = 3
Negative numbers = 2
Zero numbers = 1
```

## Concepts Used

* `for` loop
* `if-else if-else`
* `scanf()`
* `printf()`
* Comparison operators
* Increment operator `++`
* Counters

## How It Works

1. The program asks how many numbers the user wants to enter.
2. A `for` loop takes each number one by one.
3. If the number is greater than zero, the positive counter increases.
4. If the number is less than zero, the negative counter increases.
5. If the number is zero, the zero counter increases.
6. Finally, all three counts are displayed.

## C Code

```c
#include <stdio.h>

int main()
{
    int n, number;
    int positive = 0;
    int negative = 0;
    int zero = 0;

    printf("Enter how many numbers: ");
    scanf("%d", &n);

    for (int i = 1; i <= n; i++)
    {
        printf("Enter number %d: ", i);
        scanf("%d", &number);

        if (number > 0)
        {
            positive++;
        }
        else if (number < 0)
        {
            negative++;
        }
        else
        {
            zero++;
        }
    }

    printf("Positive numbers = %d\n", positive);
    printf("Negative numbers = %d\n", negative);
    printf("Zero numbers = %d", zero);

    return 0;
}
```

## Sample Output

```text
Enter how many numbers: 6
Enter number 1: 10
Enter number 2: -5
Enter number 3: 0
Enter number 4: 20
Enter number 5: -8
Enter number 6: 15

Positive numbers = 3
Negative numbers = 2
Zero numbers = 1
```

## Goal

The goal of this project is to practice loops, conditions, counters, and user input in C.
