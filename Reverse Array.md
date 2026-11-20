## 01. Reverse Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-an-array/1)

### Problem Description

**Task:** Given an array of integers arr[], reverse the array in place.Examples:Input: arr = [1, 4, 3, 2, 6, 5]

#### Examples

##### Example 1

- **Output:**
```text
[1]Explanation: The array has only single element, hence the reversed array is same as the original.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-21 02:59:00
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public void reverseArray(int arr[]) {

        int start = 0;
        int end = arr.length - 1;

        while (start < end) {

            int temp = arr[start];
            arr[start] = arr[end];
            arr[end] = temp;

            start++;
            end--;
        }
    }
}
```

*Generated on: 11/21/2026, 2:59:49 AM*