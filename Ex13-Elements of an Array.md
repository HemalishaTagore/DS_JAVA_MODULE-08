# Ex13 Fill the First 10 Elements of an Array with a Constant using Arrays.fill()
## DATE:
## AIM:
To write a Java program that fills the first 10 elements of an array with a constant value using the Arrays.fill() method.
## Algorithm

1. Start the program.
2. Create an array with more than 10 elements.
3. Use Arrays.fill() to fill the first 10 elements with the value 5.
4. Display the elements of the array.
5. Stop the program.
## Program:
```
/*
Program to fill the first 10 elements of an array with a constant value.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.Arrays;

class FillArray {

    public static void main(String[] args) {

        int arr[] = new int[15];

        Arrays.fill(arr, 0, 10, 5);

        System.out.println("Array elements:");
        System.out.println(Arrays.toString(arr));
    }
}
```

## Output:



<img width="423" height="65" alt="image" src="https://github.com/user-attachments/assets/64db8a88-57cc-4831-b295-32156e125068" />


## Result:
The program successfully fills the first 10 elements of the array with the constant value 5 using the Arrays.fill() method.
