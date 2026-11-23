## 01. Replace Consecutive Two Same with One

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/consecutive-elements2306/1)

### Problem Description

**Task:** Given a string s, consisting of lowercase alphabets. Remove consecutive duplicate characters from the string.

#### Examples

##### Example 1

- **Input:**
```text
s = "aabb"
```
- **Output:**
```text
"ab"
```
- **Explanation:** The character 'a' at index 2 is the same as 'a' at index 1, so it is removed.Similarly, the character 'b' at index 4 is the same as 'b' at index 3, so it is removed. The final string is "ab".

##### Example 2

- **Input:**
```text
s = "aabaa"
```
- **Output:**
```text
"aba"
```
- **Explanation:** The character 'a' at index 2 is the same as 'a' at index 1, so it is removed. The character 'a' at index 5 is the same as 'a' at index 4, so it is removed. The final string is "aba".

##### Example 3

- **Input:**
```text
s = "aaaa"
```
- **Output:**
```text
"a"
```
- **Explanation:** "aaaa" = > "aaa" = > "aa" = > "a"

#### Constraints

- **1.** `1 ≤ n ≤ 10⁶All characters in the string are lowercase English alphabets.`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-23 22:10:02
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public String removeDuplicates(String s) {

        StringBuilder result = new StringBuilder();

        for (int i = 0; i < s.length(); i++) {

            if (i == 0 || s.charAt(i) != s.charAt(i - 1)) {
                result.append(s.charAt(i));
            }
        }

        return result.toString();
    }
}
```

*Generated on: 11/23/2026, 10:10:30 PM*