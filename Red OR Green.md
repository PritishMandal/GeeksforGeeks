## 01. Red OR Green

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/red-or-green5711/1)

### Problem Description

**Task:** Given a string s of length n, made up of only uppercase characters 'R' and 'G', where 'R' stands for Red and 'G' stands for Green. Find the minimum number of characters need to be changed so that the entire string becomes of the same colour.Examples:Input: s = "RGRGR"

#### Examples

##### Example 1

- **Output:**
```text
1
```
- **Explanation:** We need to change only the last character to 'G' to make the string same-coloured.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-28 21:05:56
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public int redOrGreen(String s) {
         int r = 0, g = 0;

            for (int i = 0; i < s.length(); i++) {
             if (s.charAt(i) == 'R') {
                 r++;
             } else {
                 g++;
             }
         }

         return Math.min(r, g);
     }
 }
```

*Generated on: 11/28/2026, 9:09:27 PM*