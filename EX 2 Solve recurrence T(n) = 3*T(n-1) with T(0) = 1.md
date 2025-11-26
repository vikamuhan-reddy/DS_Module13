# EX 2 Solve recurrence T(n) = 3*T(n-1) with T(0) = 1

## AIM:
To write a recursive Java program to solve the recurrence relation T(n) = 3*T(n-1) with T(0) = 1.

## Algorithm
1. Start
2. Read an integer N (N ≥ 0)
3. If N = 0, return 1
4. Else, return 3 * computeT(N-1) recursively
5. Display the result
6. End

## Program:
```java
import java.util.Scanner;

public class Recurrence3Power {

    public static int computeT(int n) {
        if(n < 1) {
            return 1;
        }
        return 3 * computeT(n-1);
    }

    public static void main(String[] args) {
        Scanner scanner = new Scanner(System.in);
        int n = scanner.nextInt();

        if (n < 0) {
            System.out.println("Invalid input. n must be >= 0.");
        } else {
            int result = computeT(n);
            System.out.println("T(" + n + ") = " + result);
        }

        scanner.close();
    }
}
```

## Output:
<img width="652" height="188" alt="Screen Shot 1947-08-25 at 19 05 28" src="https://github.com/user-attachments/assets/a15ff6b0-2373-4060-b049-db465d02e4b7" />


## Result:
Thus the Java program to solve the recurrence T(n) = 3*T(n-1) with T(0) = 1 is implemented successfully.

