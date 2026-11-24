## 01. Length of String

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/length-of-string/1)

### Problem Description

**Task:** Given a string s, return the length of the string.

#### Examples

##### Example 1

- **Input:**
```text
s = "Geeks"
```
- **Output:**
```text
5
```

##### Example 2

- **Input:**
```text
s = "Hello1234"
```
- **Output:**
```text
9
```

#### Constraints

- **1.** `1 ≤ |s| ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-24 17:02:34
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public static int lengthString(String s) {
         int count = 0;

        for (int i = 0; i < s.length(); i++) {
            count++;
        }

        return count;
    }
}
```

*Generated on: 11/24/2026, 5:03:01 PM*