Enter n to generate pattern: 5
```
              1
           2  6
        3  7 10
     4  8 11 13
  5  9 12 14 15
```
solution:
```java
import java.util.*;

public class Main {
    public static void main(String[] args) {
     int n=5;
     for(int i=1;i<=n;i++){
       for(int j=1;j<=n-i;j++){
         System.out.print("    ");
       }
       int num=i;
       int diff = n-1;
       for(int j=1;j<=i;j++){
         System.out.printf("%4d",num);
         num+=diff;
         diff--;
       }
       System.out.println();
     }
  }
}

```
```
11 
7 12 
4 8 13 
2 5 9 14 
1 3 6 10 15 
```
solution
```java
public class RIghtAngleTriangleWithNumbers {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.print("Enter the n to generate pattern: ");
        int n = sc.nextInt();
        sc.close();

        for (int line = n - 1; line >= 0; line--) {
            int elementsInLine = n - line;
            for (int k = 0; k < elementsInLine; k++) {
                int diagNum = line + k;
                int startVal = (diagNum * (diagNum + 1)) / 2 + 1;
                int value = startVal + k;   
                System.out.print(value + " ");
            }
            System.out.println();
        }
    }
}

```

Given a N by M matrix of numbers, print out the matrix in a clockwise spiral.

		For example, given the following matrix:
		[[1, 2, 3, 4, 5],
		[6, 7, 8, 9, 10],
		[11, 12, 13, 14, 15],
		[16, 17, 18, 19, 20]]
		You should print out the following:
		1 2 3 4 10 15 20 19 18 17 16 11 6 7 8 9 14 13 12

Write a Java program to print the following number pattern
           
		Test Data        
		Input number of rows:  7
		Expected Output :
```
		1 2 3 4 5 6 7
		1 2 3 4 5 6
		1 2 3 4 5
		1 2 3 4
		1 2 3
		1 2 
		1 
		1 2
		1 2 3 
		1 2 3 4 
		1 2 3 4 5
		1 2 3 4 5 6
		1 2 3 4 5 6 7
```
		
Diamond pattern of stars:
```
   *
  ***
 *****
*******
 *****
  ***
   *
```

Pyramid pattern of numbers:
```
    1
   121
  12321
 1234321
123454321
```

Hour Glass Pattern
```
*********
 *    *  
  *  *   
   **    
   **    
  *  *   
 *    *  
*      * 
*********
```

Enter the string to geneate the pattern: zoho
```
z z z
 ooo 
zo.ho
 hhh 
o o o
```

Enter the string to geneate the pattern: hello
```
h h h
 eee 
hello
 lll 
o o o
```



