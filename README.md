## contributions are welcomed!!!
Enter n to generate pattern: 5
```
  1  2  3  4  5
 10  9  8  7  6
 11 12 13 14 15
 20 19 18 17 16
 21 22 23 24 25
```
Solution:
```java
public class Main {
    public static void main(String[] args) {
        int n = 5;
        int num = 1;

        for (int i = 1; i <= n; i++) {
            if (i % 2 == 1) {  
                for (int j =1 ; j <= n; j++) {
                    System.out.printf("%3d", num++);
                }
            } else {           
                int start = num + n -1;
                for(int j=1;j<=n;j++){
                  System.out.printf("%3d", start--);
                }
                num+=n;
            }
            System.out.println();
        }
    }
}

```
Enter n to generate pattern: 5
```
1 2 3 4 5 
5 1 2 3 4 
4 5 1 2 3 
3 4 5 1 2 
2 3 4 5 1
```
Solution:
```java
 class Main {
    public static void main(String[] args) {
      int n=5;
      for(int i=1;i<=n;i++){
        int num = 5-i+1;
        for(int j=1;j<i;j++){
          System.out.print(++num+" ");
        }
        for(int j=1;j<=n-i+1;j++){
          System.out.print(j+" ");
        }
        System.out.println();
      }
  }
}
```
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
       int n=5;
       for(int line = n-1;line>=0;line--){
         // no of elements to be printed in a line
         int noOfEle = n - line;
         for(int k=0;k<noOfEle;k++){
           // upto n we sum using (n*(n+1))/2 formula and adding 1 and k to match the pattern
           int upToSumNum = line + k;
           int sum = (upToSumNum *(upToSumNum+1))/2+1;
           int finalValue = sum + k;
           System.out.printf("%-3d",finalValue);
         }
         System.out.println();
       }
    }
}

```

Given a N by M matrix of numbers, print out the matrix in an  anit-clockwise spiral.
![matrix printin](https://github.com/Magesh-sam/zoho-patterns/blob/main/matrixprinting.png)

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
Solution:
```java
public class Main {
    public static void main(String[] args) {
      int n=7;
     for(int i=1;i<=n;i++){
       for(int j=1;j<=n-(i-1);j++){
         System.out.print(j);
       }
       System.out.println();
     }
     for(int i=2;i<=n;i++){
       for(int j=1;j<=i;j++){
         System.out.print(j);
       }
       System.out.println();
     }
  }
}
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
Solution:
```java
public void pattern9(int n) {
        for(int i=1;i<=n;i++){
            for(int j=1;j<=n-i;j++){
                System.out.print(" ");
            }
            for(int j=1;j<=((2*i)-1);j++){
                System.out.print("*");
            }
            System.out.println();
        }
        for(int i=1;i<=n-1;i++){
        //spaces
        for(int j=1;j<=i;j++){
          System.out.print(" ");
        }
        //stars
        for(int j=1;j<(2*n-1)-((2*i)-1);j++){
          System.out.print("*");
        }
        System.out.println();
      }
    }
```

Pyramid pattern of numbers:
```
    1
   121
  12321
 1234321
123454321
```
Solution:
```java
public class Main {
    public static void main(String[] args) {
      int n=5;
     for(int i=1;i<=n;i++){
       
       for(int j=1;j<=n-i;j++){
         System.out.print(" ");
       }
       
       for(int j=1;j<=i;j++){
         
         System.out.print(j);
       }
       
       for(int j=i-1;j>=1;j--){
         System.out.print(j);
         
       }
       System.out.println();
     }
     
  }
}
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



