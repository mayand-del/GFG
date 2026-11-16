## 01. Perfect Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/perfect-numbers3207/1)

### Problem Description

**Task:** Given a number n, check if the number is perfect or not. A number is said to be perfect if sum of all its factors excluding the number itself is equal to the number.Examples:Input: n = 6

#### Examples

##### Example 1

- **Output:**
```text
falseExplanation: Factors of 15 are 1, 3, 5, 15. Excluding 15 their sum is 9 which is not equal to n itself. So, it's not a Perfect Number.
```
- **Explanation:** Factors of 6 are 1, 2, 3 and 6. Excluding 6 their sum is 6 which is equal to n itself. So, it's a Perfect Number.Input: n = 10

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-16 21:32:04
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    static boolean isPerfect(int n) {
        // code here
        int sum=0;
        for(int i=1;i*i<=n;i++){
            if(n%i==0){
                sum+=i;
                if(i != 1 && i != n / i) {
                     sum += n / i;
                }
            }
        }
        return sum==n;
    }
};
```

*Generated on: 16/11/2026, 21:32:36*