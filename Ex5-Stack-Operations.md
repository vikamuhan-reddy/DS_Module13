# EX 5 Implement Bubble Sort to Sort an Array in Ascending Order

## AIM:
To write a Java program to sort an unsorted array in ascending order using the Bubble Sort algorithm.

## Algorithm
1. Start  
2. Read the number of elements N  
3. Read the elements of the array  
4. Loop through the array N-1 times  
5. Compare adjacent elements and swap if the first is greater than the second  
6. Repeat until the array is sorted  
7. Print the sorted array  
8. End

## Program:
```java
import java.util.Scanner;

class prog {
    
    static void bubbleSort(int arr[], int n){
        for (int i = 0; i < n - 1; i++) {
            for (int j = 0; j < n - 1 - i; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }

    // Function to print an array
    static void printArray(int arr[], int size){
        for (int i = 0; i < size; i++)
            System.out.print(arr[i] + " ");
        System.out.println();
    }

    // Driver program
    public static void main(String args[]){
        Scanner sc = new Scanner(System.in);
        int n = sc.nextInt();
        
        int arr[] = new int[n];
        for(int i = 0; i < n; i++){
            arr[i] = sc.nextInt();
        }
        bubbleSort(arr, n);
       
        printArray(arr, n);
    }
}
```


## Output:
<img width="487" height="225" alt="Screen Shot 1947-08-25 at 19 14 16" src="https://github.com/user-attachments/assets/b0667522-445a-467e-a60d-fc3fd9b8110f" />


## Result:
Thus the Java program to sort an unsorted array in ascending order using Bubble Sort is implemented successfully.

