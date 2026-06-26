# String Encryption in C

This C program demonstrates a simple string encryption technique by increasing the ASCII value of every character in a string by **1**.

## How It Works

- A character array (string) is initialized.
- The `strlen()` function is used to determine the length of the string.
- A `for` loop traverses each character of the string.
- Each character's ASCII value is increased by `1`.
- The modified (encrypted) string is printed.

## Code

```c
#include <stdio.h>
#include <string.h>

int main() {
    char st[] = "Aaj to monday hai";

    for (int i = 0; i < strlen(st); i++) {
        st[i] = st[i] + 1;
    }

    printf("%s", st);

    return 0;
}
```

## Example

### Input

```
Aaj to monday hai
```

### Output

```
Bbk!up!npoebz!ibj
```

## ASCII Conversion Example

| Original Character | ASCII | Encrypted Character | ASCII |
|--------------------|------:|--------------------|------:|
| A | 65 | B | 66 |
| a | 97 | b | 98 |
| j | 106 | k | 107 |
| Space | 32 | ! | 33 |

## Concepts Used

- Strings in C
- Character Arrays
- `strlen()` Function
- `for` Loop
- ASCII Character Encoding

## Time Complexity

- **O(n²)** (because `strlen()` is called in every loop iteration)

> **Note:** A more efficient approach is to store the result of `strlen(st)` in a variable before the loop, reducing the time complexity to **O(n)**.

## Learning Outcome

This program helps understand:

- How strings are stored in C.
- How `strlen()` determines the length of a string.
- How characters are internally represented using ASCII values.
- How simple character-based encryption techniques work.
