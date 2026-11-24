## 01. First Letter of Every Word

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/print-first-letter-of-every-word-in-the-string3632/1)

### Problem Description

**Task:** Given a string s, the task is to create a string with the first letter of every word in the string. The string s contains lower case English alphabets and its words have a single space between them.

#### Examples

##### Example 1

- **Input:**
```text
s = "geeks for geeks"
```
- **Output:**
```text
gfgExplanation: First word starts at index 0, take 'g' After first space, next word starts with 'f'After second space, next word starts with 'g'
```

##### Example 2

- **Input:**
```text
s = "bad is good"
```
- **Output:**
```text
big
```

#### Constraints

- **1.** `1 ≤ |s| ≤ 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(|S|)
- **Expected Auxiliary Space Complexity:** O(|S|)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-24 21:30:12
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    String firstAlphabet(String s) {
              StringBuilder ans = new StringBuilder();

                ans.append(s.charAt(0));

                for (int i = 1; i < s.length(); i++) {

                    if (s.charAt(i) == ' ') {
                        ans.append(s.charAt(i + 1));
                    }
                }

                return ans.toString();
        
    }
};
```

*Generated on: 11/24/2026, 9:31:23 PM*