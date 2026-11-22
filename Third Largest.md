## 01. Third Largest

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/third-largest-element/1)

### Problem Description

**Task:** Given an array, arr[] of positive integers. Find the third largest element in it. Return -1 if the third largest element is not found.Examples:Input: arr[] = [2, 4, 1, 3, 5]Output: 3Explanation: The third largest element in the array [2, 4, 1, 3, 5] is 3.Input: arr[] = [10, 2]Output: -1Explanation: There are less than three elements in the array, so the third largest element cannot be determined.Input: arr[] = [5, 5, 5]Output: 5Explanation: In the array [5, 5, 5], the third largest element can be considered 5, as there are no other distinct elements.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-22 15:06:12
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int thirdLargest(List<Integer> arr) {

        if(arr.size() < 3) {
            return -1;
        }

        int first = -1;
        int second = -1;
        int third = -1;

        for(int i = 0; i < arr.size(); i++) {

            if(arr.get(i) >= first) {
                third = second;
                second = first;
                first = arr.get(i);
            }
            else if(arr.get(i) >= second) {
                third = second;
                second = arr.get(i);
            }
            else if(arr.get(i) >= third) {
                third = arr.get(i);
            }
        }

        return third;
    }
}
```

*Generated on: 11/22/2026, 3:06:42 PM*