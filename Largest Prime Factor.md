## 01. Largest Prime Factor

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/largest-prime-factor2601/1)

### Problem Description

**Task:** Given a number n, your task is to find the largest prime factor of n.

#### Examples

##### Example 1

- **Input:**
```text
n = 5
```
- **Output:**
```text
5
```
- **Explanation:** The prime factorization of 5 is just 5. Therefore, the largest prime factor is 5.

##### Example 2

- **Input:**
```text
n = 24
```
- **Output:**
```text
3
```
- **Explanation:** The prime factorization of 24 is 2³×3. Among the prime factors (2, 3), the largest is 3.

##### Example 3

- **Input:**
```text
n = 13195
```
- **Output:**
```text
29
```
- **Explanation:** The prime factorization of 13195 is 5×7×13×29. The largest prime factor is 29.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(sqrt(n))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-04 23:40:23
- **Status:** Correct
- **Marks:** 4

```java
class Solution {
    static int largestPrimeFactor(int n) {

                int ans = 1;

                for(int i = 2; i * i <= n; i++) {
                    while(n % i == 0) {
                        ans = i;
                        n = n / i;
                    }
                }

                if(n > 1) {
                    ans = n;
                }

                return ans;
            }
        }
```

*Generated on: 04/11/2026, 23:40:52*