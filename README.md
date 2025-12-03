# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```
#include <stdio.h>

int main() {
    long a = 1103515245;   // multiplier
    long c = 12345;        // increment
    long m = 32768;        // modulus
    long seed, next;

    printf("Enter the seed value: ");
    scanf("%ld", &seed);

    printf("\nPseudo Random Numbers:\n");

    next = seed;

    for (int i = 0; i < 10; i++) {     // generate 10 numbers
        next = (a * next + c) % m;
        printf("%ld ", next);
    }

    printf("\n");
    return 0;
}

```
# OUTPUT:
<img width="1730" height="545" alt="image" src="https://github.com/user-attachments/assets/e84135b4-788c-4511-ae16-302eac80bb77" />

# RESULT:
