## 01. Learn to Comment

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/learn-to-comment/1)

### Problem Description

**Task:** Given three lines that print the values of a, b, and c. comment out the line that prints the value of b.Comments are useful in any programming language to describe the purpose of functions or operations. They are ignored by the compiler, so they do not affect the execution of the code.Examples: Input: a = 5, b = 6, c = 15

#### Examples

##### Example 1

- **Explanation:** 5 15Input:a = 6, b = 8, c = 10 6 10

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-20 12:42:40
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int b = sc.nextInt();
        int c = sc.nextInt();

        // Prints a
        System.out.println(a);

        // Prints b
        //System.out.println(b);

        // Prints c
        System.out.println(c);
    }
}
```

*Generated on: 20/11/2026, 12:43:55*