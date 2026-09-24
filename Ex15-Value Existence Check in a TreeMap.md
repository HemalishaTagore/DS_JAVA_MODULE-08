# Ex15 Value Existence Check in a TreeMap
## DATE: 20/08/2026
## AIM:
To write a Java program that checks whether a given value exists in a TreeMap.

## Algorithm
1. Start the program.
2. Create a TreeMap and add key-value pairs.
3. Read the value to be searched.
4. Use the containsValue() method to check whether the value exists in the TreeMap.
5. Display the result and stop the program.

## Program:
```
/*
Program to check whether a given value exists in a TreeMap.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.*;

class TreeMapValueCheck {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        TreeMap<Integer, String> map = new TreeMap<>();

        map.put(1, "Apple");
        map.put(2, "Banana");
        map.put(3, "Mango");
        map.put(4, "Orange");

        System.out.println("TreeMap: " + map);

        System.out.print("Enter value to search: ");
        String value = sc.nextLine();

        if (map.containsValue(value))
            System.out.println("Value exists in the TreeMap.");
        else
            System.out.println("Value does not exist in the TreeMap.");

        sc.close();
    }
}
```

## Output:
<img width="1025" height="761" alt="image" src="https://github.com/user-attachments/assets/719cc1fb-0198-431c-b1dd-a78fb23676d9" />



## Result:
Thus, the program successfully checks whether a specified value exists in a TreeMap using the containsValue() method.
