## 01. Calculator

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/calculator--172632/1)

### Problem Description

**Task:** Given two numbers a and b. You need to perform basic mathematical operations on them. You will be provided an integer named as optr. If the operator equals to 1 add a and b, then print the result.If the operator equals to 2 subtract b from a, then print the result.If the operator equals to 3 multiply a and b, then print the result.If the operator equals to any other number, print "Invalid Input"(without quotes).Note: Do not add a new line at the end.Examples:Input: a = 1, b = 2, optr = 3

#### Examples

##### Example 1

- **Output:**
```text
0
```
- **Explanation:** 2 - 2 = 0

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-23 21:36:52
- **Status:** Correct
- **Marks:** 2

```java
class Solution {
    public void calculate(int a, int b, int optr) {
        switch(optr){
            case 1:
                System.out.print(a+b);
                break;
                
            case 2:
                System.out.print(b-a);
                break;
                
            case 3:
                System.out.print(a*b);
                break;
                
            default:
            System.out.println("Invalid Input");
        }
    }
}
```

*Generated on: 23/11/2026, 21:37:21*