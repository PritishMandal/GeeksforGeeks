## 01. Smallest in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/vector-min-element--151110/1)

### Problem Description

**Task:** Given an array of integers arr[]. Find the minimum element in the array using you language's inbuilt function.Examples:Input: arr[] = [1, 2, 3, 4]Output: 1Input: arr[] = [3, 2, 1]Output: 1Input: arr[] = [5, 4, 2, 8, 8]Output: 2

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-27 23:24:04
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int findMin(int[] arr) {
               return Arrays.stream(arr).min().getAsInt();
        
    }
}
```

*Generated on: 11/27/2026, 11:24:30 PM*