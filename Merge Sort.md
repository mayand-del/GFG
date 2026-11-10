## 01. Merge Sort

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/merge-sort/1)

### Problem Description

**Task:** Given an array arr[], its starting position l and its ending position r. Sort the array using the merge sort algorithm.Examples:Input: arr[] = [4, 1, 3, 9, 7]

#### Examples

##### Example 1

- **Output:**
```text
[1, 3, 4, 7, 9]Explanation: We get the sorted array after using merge sort
```

##### Example 2

- **Input:**
```text
arr[] = [10, 9, 8, 7, 6, 5, 4, 3, 2, 1]
```
- **Output:**
```text
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]Explanation: We get the sorted array after using merge sort
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n log n)
- **Expected Auxiliary Space Complexity:** O(n)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-10 19:37:59
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    public void mergeSort(int arr[], int l, int r) {
        // code here
        if(l>=r){
            return;
        }
        int mid=l+(r-l)/2;
        mergeSort(arr,l,mid);
        mergeSort(arr,mid+1,r);
        merge(arr,l,mid,r);
    }
    public static void merge(int arr[],int l,int mid,int r){
        int temp[]=new int[r-l+1];
        int i=l;
        int j=mid+1;
        int k=0;
        
        while(i<=mid && j<=r){
            if(arr[i]<arr[j]){
                temp[k]=arr[i];
                i++;
            }else{
                temp[k]=arr[j];
                j++;
            }
            k++;
        }
        
        while(i<=mid){
            temp[k++]=arr[i++];
        }
        
        while(j<=r){
            temp[k++]=arr[j++];
        }
        
        for(k=0,i=l;k<temp.length;k++,i++){
            arr[i]=temp[k];
        }
    }
}
```

*Generated on: 10/11/2026, 19:38:55*