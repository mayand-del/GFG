## 01. Even Odd Game

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/even-odd-game--153136/1)

### Problem Description

**Task:** Given a number n, number of apples in a bag. You and your friend are picking one apple turnwise from the bag. It is given that the first attempt is always by you. The person picking the last apple will be the winner.
If you will win: print "You" (without quotes)
If your friend will win: print "Friend" (without quotes)

#### Examples

##### Example 1

- **Input:**
```text
n = 9
```
- **Output:**
```text
You
```

##### Example 2

- **Input:**
```text
n = 4
```
- **Output:**
```text
Friend
```

#### Constraints

- **1.** `1 ≤ n ≤ 100`

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-22 14:47:25
- **Status:** Correct
- **Marks:** 2

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        // code here
        if(n%2==0){
            System.out.println("Friend");
        }else{
            System.out.println("You");
        }

        sc.close();
    }
}
```

*Generated on: 22/11/2026, 14:47:54*