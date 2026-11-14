## 01. Vowel or Not

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/vowel-or-not0831/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given a character ch representing an English alphabet, determine whether it is a vowel or not. Return true if ch is a vowel otherwise return false.

#### Examples

##### Example 1

- **Input:**
```text
ch = 'a'
```
- **Output:**
```text
trueExplanation: 'a' is a vowel. So output for this test case is true.
```

##### Example 2

- **Input:**
```text
ch = 'Z'
```
- **Output:**
```text
falseExplanation: 'Z' is not a vowel. So output for this test case is false.
```

#### Constraints

- **1.** `ch is a lowercase or uppercase English letter.`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-14 20:36:29
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        char ch = sc.next().charAt(0);

        if (ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u' ||
            ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U') {
            System.out.println("true");
        } else {
            System.out.println("false");
        }
    }
}
```

*Generated on: 11/14/2026, 8:37:08 PM*