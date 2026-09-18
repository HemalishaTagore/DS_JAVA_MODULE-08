# Ex12 Add Elements from an Array into a TreeSet
## DATE:
## AIM:
To write a Java program that adds elements from an array into a TreeSet and displays the elements in sorted order.
## Algorithm
1. Start the program.
2. Read the elements of an array.
3. Create a TreeSet and add all array elements into it.
4. Display the elements of the TreeSet in sorted order.
5. Stop the program.

## Program:
```
/*
Program to add elements from an array into a TreeSet.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.*;

class ArrayToTreeSet {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        int arr[] = new int[n];

        System.out.println("Enter array elements:");
        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        TreeSet<Integer> set = new TreeSet<>();

        for (int i = 0; i < n; i++) {
            set.add(arr[i]);
        }

        System.out.println("TreeSet elements in sorted order:");
        System.out.println(set);

        sc.close();
    }
}
```

## Output:
<img width="300" height="262" alt="image" src="https://github.com/user-attachments/assets/f77dbe87-9909-45b3-bf08-059d73c67250" />



## Result:
The program successfully adds elements from an array into a TreeSet.
