# EX 3 Compute the Factorial of a Number using Recursion and Iteration

## AIM:
To write a Java program to compute the factorial of a number using both recursion and iteration.

## Algorithm
1. Start
2. Read an integer N
3. If N < 0, display error (factorial not defined)
4. Else, calculate factorial recursively
5. Calculate factorial iteratively
6. Display both results
7. End

## Program:
```java
import java.util.Scanner;

public class FactorialCalculator {

    // Recursive method to calculate factorial
    static long factorialRecursive(int n) {
        if(n == 0){
            return 1;
        }
        return n * factorialRecursive(n-1);
    }

    // Iterative method to calculate factorial
    static long factorialIterative(int n) {
        int answer = 1;
        for(int i = 1; i <= n; i++){
            answer *= i;
        }
        return answer;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        
        int num = sc.nextInt();
        
        if (num < 0) {
            System.out.println("Factorial is not defined for negative numbers.");
        } else {
            System.out.println("Factorial (Recursive): " + factorialRecursive(num));
            System.out.println("Factorial (Iterative): " + factorialIterative(num));
        }
    }
}
```

## Output:
<img width="590" height="229" alt="Screen Shot 1947-08-25 at 19 08 54" src="https://github.com/user-attachments/assets/a6b824df-fc53-4070-a5c0-262d47ce5129" />


## Result:
Thus the Java program to compute the factorial of a number using recursion and iteration is implemented successfully.

