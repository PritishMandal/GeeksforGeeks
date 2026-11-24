## 01. Nth Number with Prime Digits

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/nth-number-made-of-prime-digits4319/1)

### Problem Description

**Task:** Given a number n. You have to find the n^th number whose each digit is a prime number i.e. 2, 3, 5, 7. In other words, you have to find nth number of this sequence: 2, 3, 5, 7, 22, 23 ,... and so on.Examples:Input: n = 10

#### Examples

##### Example 1

- **Output:**
```text
33
```
- **Explanation:** 10^th number in the sequence of numbers whose each digit is prime is 33.

##### Example 2

- **Input:**
```text
n = 21
```
- **Output:**
```text
222
```
- **Explanation:** The 21^st number in the sequence of numbers whose each digit is prime is 222.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(log n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-24 21:14:17
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public int primeDigits(int n) {

                String digits = "2357";
                StringBuilder ans = new StringBuilder();

                n--;

                while(n >= 0) {
                      ans.append(digits.charAt(n % 4));
                    n = n / 4;
                      if(n == 0)
                        break;

                    n--;
                }

                return Integer.parseInt(ans.reverse().toString());
            }
        
}
```

*Generated on: 11/24/2026, 9:44:36 PM*