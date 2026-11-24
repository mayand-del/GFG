## 01. The FizzBuzz Program

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/the-fizzbuzz-program/1)

### Problem Description

**Task:** Given a number n, print your answer according to the following conditions:If the number is divisible by 3, you print FizzIf the number is divisible by 5, you print BuzzIf the number is divisible by both 3 and 5, you print FizzBuzzIn any other case, you print the number itselfExamples:Input: n = 3

#### Examples

##### Example 1

- **Output:**
```text
7
```
- **Explanation:** 7 is not divisible by 3 or 5.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (Java)

- **Submitted:** 2026-11-24 12:41:05
- **Status:** Correct
- **Marks:** 2

```java
import java.util.Scanner;

class GFG {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();

        // code here
        // if(n%3==0){
        //     System.out.println("Fizz");
        // } else if(n%5==0){
        //     System.out.println("Buzz");
        // }else if(n%3==0 && n%5==0){
        //     System.out.println("FizzBuzz");
        // }else{
        //     System.out.print(n);
        // }
        if(n%3==0 && n%5==0){
            System.out.println("FizzBuzz");
        }
        else if(n%3==0){
            System.out.println("Fizz");
        }
        else if(n%5==0){
            System.out.println("Buzz");
        }
        else{
            System.out.println(n);
        }
    }
}
```

*Generated on: 24/11/2026, 12:41:43*