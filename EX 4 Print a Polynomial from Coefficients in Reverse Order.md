# EX 4 Print a Polynomial from Coefficients in Reverse Order

## AIM:
To write a Java program to read the degree and coefficients of a polynomial and print the polynomial in standard form.

## Algorithm
1. Start  
2. Read the degree of the polynomial N  
3. Create an array of size N+1 to store coefficients  
4. Read the coefficients from degree 0 to N  
5. Loop from N down to 0 and print each term in the format `coefficient*x^degree`  
6. End

## Program:
```java
import java.util.Scanner;

public class poly {
    public static void main(String[] args){
        Scanner sc = new Scanner(System.in);
        
        int n = sc.nextInt();
        int[] arr = new int[n+1];
        
        for(int i = 0; i <= n; i++){
            arr[i] = sc.nextInt();
        }
        for(int i = n; i >= 0; i--){
            System.out.print(arr[i] + "x^" + i);
            if(i > 0){
                System.out.print(" + ");
            }
        }
    }
}

```

## Output:
<img width="696" height="273" alt="Screen Shot 1947-08-25 at 19 11 07" src="https://github.com/user-attachments/assets/18099830-8861-449d-bbce-9842513b7d06" />


## Result:
The loop is printed in reverse order (from highest degree to lowest) because in standard polynomial notation, the highest degree term comes first.
Thus the Java program to read coefficients and print the polynomial in standard form is implemented successfully.

