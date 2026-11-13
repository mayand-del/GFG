## 01. First Occurrence in Sorted

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/binary-search-1587115620/1)

### Problem Description

**Task:** Given a sorted array arr[] and an integer k, find the position(0-based indexing) at which k is present in the array using binary search. If k doesn't exist in arr[] return -1. Note: If multiple occurrences are there, please return the smallest index.Examples:Input: arr[] = [1, 2, 3, 4, 5], k = 4

#### Examples

##### Example 1

- **Output:**
```text
0
```
- **Explanation:** 1 appears at index 0.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-13 15:37:04
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public int firstSearch(int[] arr, int k) {
        int low=0;
        int high=arr.length-1;
        int ans=-1;
        while(low<=high){
            int mid=low+(high-low)/2;
            if(arr[mid]==k){
                ans=mid;
                high=mid-1;
                
            }else if(arr[mid]<k){
                low=mid+1;
            }else{
                high=mid-1;
            }
        }
        return ans;
    }
}
```

*Generated on: 13/11/2026, 15:37:36*