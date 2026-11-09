## 01. Two Sum - Pair with Given Sum

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/key-pair5616/1)

### Problem Description

**Task:** Given an array arr[] of integers and another integer target. Determine if there exist two distinct indices such that the sum of their elements is equal to the target.Examples:Input: arr[] = [0, -1, 2, -3, 1], target = -2

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** No pair is possible as only one element is present in arr[]

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-09 08:09:43
- **Status:** Correct
- **Marks:** 2

```java
import java.util.*;

class Solution {
    static boolean twoSum(int arr[], int target) {

        int[] nums = arr.clone();
        Arrays.sort(nums);

        int left = 0;
        int right = nums.length - 1;

        while (left < right) {

            int sum = nums[left] + nums[right];

            if (sum == target) {
                return true;
            }
            else if (sum < target) {
                left++;
            }
            else {
                right--;
            }
        }

        return false;
    }
}
```

*Generated on: 11/9/2026, 8:10:14 AM*