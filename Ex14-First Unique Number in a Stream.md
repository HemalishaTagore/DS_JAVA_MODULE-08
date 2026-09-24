# Ex14 Tracking the First Unique Number in a Stream using LinkedHashMap
## DATE: 20/08/2026
## AIM:
To implement a program that tracks the first unique (non-repeating) number in a stream of integers using a LinkedHashMap.

## Algorithm

1. Start the program.
2. Read the stream of integers and store their frequency using LinkedHashMap.
3. Traverse the LinkedHashMap in insertion order.
4. Find the first element whose frequency is 1.
5. Display the first unique number and stop the program.
## Program:
```
/*
Program to track the first unique number in a stream using LinkedHashMap.
Developed by: HEMALISHA T
RegisterNumber: 212225040123
*/

import java.util.*;

class FirstUniqueNumber {

    public static void main(String[] args) {

        Scanner sc = new Scanner(System.in);

        LinkedHashMap<Integer, Integer> map = new LinkedHashMap<>();

        System.out.print("Enter number of elements: ");
        int n = sc.nextInt();

        System.out.println("Enter stream elements:");

        for (int i = 0; i < n; i++) {
            int num = sc.nextInt();
            map.put(num, map.getOrDefault(num, 0) + 1);
        }

        int firstUnique = -1;

        for (Map.Entry<Integer, Integer> entry : map.entrySet()) {
            if (entry.getValue() == 1) {
                firstUnique = entry.getKey();
                break;
            }
        }

        if (firstUnique != -1)
            System.out.println("First unique number: " + firstUnique);
        else
            System.out.println("No unique number found.");

        sc.close();
    }
}
```

## Output:


<img width="696" height="622" alt="image" src="https://github.com/user-attachments/assets/7fd6327e-d538-42d3-841e-402a682c8ec3" />


## Result:
The program successfully tracks and returns the first unique number at any point in the integer stream using a LinkedHashMap.
