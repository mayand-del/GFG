## 01. Search in Rotated Sorted Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/search-in-a-rotated-array4618/1)

### Problem Description

**Task:** Given an array arr[] of distinct elements, which was initially sorted in ascending order but then rotated at some unknown pivot, the task is to find the index of a target key. If the key is not present in the array, return -1.Examples :Input: arr[] = [5, 6, 7, 8, 9, 10, 1, 2, 3], key = 3

#### Examples

##### Example 1

- **Output:**
```text
1
```
- **Explanation:** 42 is found at index 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-12 16:17:50
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    int search(int arr[],int key){
        return search(arr,key,0,arr.length-1);
    }
    int search(int[] arr, int key, int si, int ei) {
        if(si > ei) {
            return -1;
        }

        int mid = si + (ei - si) / 2;

        if(arr[mid] == key) {
            return mid;
        }

        if(arr[si] <= arr[mid]) {
            if(arr[si] <= key && key < arr[mid]) {
                return search(arr, key, si, mid - 1);
            } else {
                return search(arr, key, mid + 1, ei);
            }
        } else {
            if(arr[mid] < key && key <= arr[ei]) {
                return search(arr, key, mid + 1, ei);
            } else {
                return search(arr, key, si, mid - 1);
            }
        }
    }
}
```

*Generated on: 12/11/2026, 16:18:22*