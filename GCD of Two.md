## 01. GCD of Two

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/gcd-of-two-numbers3459/1)

### Problem Description

**Task:** Given two positive integers a and b, find GCD of a and b.

> **Note:** Don't use the inbuilt gcd function

#### Examples

##### Example 1

- **Input:**
```text
a = 20, b = 28
```
- **Output:**
```text
4
```
- **Explanation:** GCD of 20 and 28 is 4

##### Example 2

- **Input:**
```text
a = 60, b = 36
```
- **Output:**
```text
12
```
- **Explanation:** GCD of 60 and 36 is 12

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log(min(a, b)))
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-17 15:28:57
- **Status:** Correct
- **Marks:** 1

```java
class Solution {
    public static int gcd(int a, int b) {
        
        while(b!=0){
            int c=a%b;
            a=b;
            b=c;
        }
        return a;
    }
}
```

*Generated on: 17/11/2026, 15:29:28*