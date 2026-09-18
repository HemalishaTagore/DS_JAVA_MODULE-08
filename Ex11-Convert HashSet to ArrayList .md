# Ex11 Convert HashSet to ArrayList in Java
## DATE:
## AIM:
To convert a collection of distinct integers stored in a HashSet into an ArrayList and display its contents.
## Algorithm
1. Start the program.
2. Create a HashSet and add distinct integer elements.
3. Create an ArrayList using the HashSet.
4. Display the elements of the ArrayList.
5. Stop the program.

## Program:
```
/*
Program to convert a HashSet into an ArrayList.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.*;

class HashSetToArrayList {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        HashSet<Integer> set = new HashSet<>();

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        System.out.println("Enter elements:");
        for (int i = 0; i < n; i++) {
            set.add(sc.nextInt());
        }

        ArrayList<Integer> list = new ArrayList<>(set);

        System.out.println("ArrayList elements:");
        System.out.println(list);

        sc.close();
    }
}
```

## Output:

<img width="264" height="241" alt="image" src="https://github.com/user-attachments/assets/c30452af-7968-4494-aa69-b64aad7fc3fe" />


## Result:
The program successfully converts a collection of distinct integers stored in a HashSet into an ArrayList
