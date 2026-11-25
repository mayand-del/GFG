## 01. AP Term

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/ap-term--150919/1)

### Problem Description

**Task:** Given three integers a, d and n. Where a is the first term, d is the common difference of an A.P. Calculate the n_th_ term of A.P. The n_th term is given by a_n = a + (n-1)d

#### Examples

##### Example 1

- **Input:**
```text
a = 5, d = 2, n = 5
```
- **Output:**
```text
13
```
- **Explanation:** a_nth = a + (n-1)d = 5 + (5-1)*2 = 5 + 8 = 13

##### Example 2

- **Input:**
```text
a = 10, d = 10, n = 101
```
- **Output:**
```text
1010
```
- **Explanation:** a_nth = a + (n-1)d = 10 + (101-1)*10 = 10 + 1000 = 1010.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-25 12:15:33
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();
        int d = sc.nextInt();
        int n = sc.nextInt();

        // code here
        int anth=a + (n-1)*d;
        System.out.println(anth);
    }
}
```

*Generated on: 25/11/2026, 12:16:10*