## 01. Quick Sort

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/quick-sort/1)

### Problem Description

**Task:** Given an array arr[], with starting index low and ending index high, complete the functions partition() and quickSort() so that the array becomes sorted in ascending order.Examples:Input: arr[] = [4, 1, 3, 9, 7]

#### Examples

##### Example 1

- **Output:**
```text
[5, 5, 5, 5]Explanation: All elements are identical, so the array remains unchanged.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-11 17:23:16
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public void quickSort(int[] arr, int low, int high) {
        if(low>=high){
            return;
        }
        
        int pidx=partition(arr,low,high);
        quickSort(arr,low,pidx-1);
        quickSort(arr,pidx+1,high);
        
    }

    private int partition(int[] arr, int low, int high) {
        int pivot=arr[high];
        int i=low-1;
        for(int j=low;j<high;j++){
            if(arr[j]<=pivot){
                i++;
                int temp=arr[j];
                arr[j]=arr[i];
                arr[i]=temp;
            }
        }
        i++;
        int temp=pivot;
        arr[high]=arr[i];
        arr[i]=temp;
        return i;
        
    }
}
```

*Generated on: 11/11/2026, 17:23:53*