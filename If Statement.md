## 01. If Statement

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/the-if-statement--113256/1)

### Problem Description

**Task:** Given a number n, use the if statement to print "Big" (without quotes) if the given number is greater than 100. The statement "Number" (without quotes) will be printed regardless.Note: Follow Sample cases for the output format. After printing move the cursor to the next line.Examples :Input: n = 10

#### Examples

##### Example 1

- **Output:**
```text
Number
```
- **Explanation:** 10 is less than 100, so we don't print Big and Number will be printed by default.

##### Example 2

- **Input:**
```text
n = 101
```
- **Output:**
```text
Big Number
```
- **Explanation:** 101 is greater than 100, so we print Big and Number will be printed by default in the next line.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-19 15:00:50
- **Status:** Correct
- **Marks:** 1

```java
import java.util.*;

public class Solution {
    public static void solve() {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        // code here
        if(n>100){
            System.out.println("Big\nNumber");
        }else{
            System.out.print("Number");
        }
    }
}
```

*Generated on: 19/11/2026, 15:01:17*