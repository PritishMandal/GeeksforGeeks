## 01. Sum Of Digits

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/sum-of-digits1742/1?utm_source=chatgpt.com)

### Problem Description

**Task:** Given a positive number n. Find the sum of all the digits of n.

#### Examples

##### Example 1

- **Input:**
```text
n = 687
```
- **Output:**
```text
21
```
- **Explanation:** Sum of 687's digits: 6 + 8 + 7 = 21

##### Example 2

- **Input:**
```text
n = 12 Output 3
```
- **Explanation:** Sum of 12's digits: 1 + 2 = 3

#### Constraints

- **1.** `1 <= n <= 10⁵`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-13 12:50:10
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    static int sumOfDigits(int n) {
        // code here
        int sum = 0;
     
    
        while(n>0){
            int digit = n % 10;
            sum += digit;
            n/= 10;
        }
        return sum;
    }
}
```

*Generated on: 11/13/2026, 12:51:19 PM*