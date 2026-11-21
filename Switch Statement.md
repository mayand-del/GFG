## 01. Switch Statement

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/switch-statement/1)

### Problem Description

**Task:** Given a number n, use a switch statement to print "Stop" if the given number is 1 (or Red light)"Standby" if the number is 2 (Yellow light)"Go" if the number is 3 (Green light). For any other number, print "Unknown" (without quotes).Examples:Input: n = 1

#### Examples

##### Example 1

- **Output:**
```text
Unknown
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-21 15:08:08
- **Status:** Correct
- **Marks:** 1

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        // code here
        switch(n){
            case 1:
                System.out.println("Stop");
                break;
            case 2:
                System.out.println("Standby");
                break;
            case 3:
                System.out.println("Go");
                break;
                
            default:
                  System.out.println("Unknown");
                
        }
    }
}
```

*Generated on: 21/11/2026, 15:08:34*