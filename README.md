# Wipro-Tech-Training-
Harshad number

Write a program to find whether the given number is a Harshad number or not. Note that Harshard number is an integer that is divisible by the sum of its digits.

# Input Format

Input consists of 1 integer.

# Constraints

No Constraints

# Output Format

If the given number is a Harshad Number, display “Harshad Number” or display “Not Harshad Number”.

# Sample Input 0

11
# Sample Output 0

Not Harshad Number
Sample Input 1

1729
Sample Output 1

# Harshad Number

import java.io.*;
import java.util.*;

public class Solution {

    public static void main(String[] args) {
    Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int sum=0;
        int temp=n;
        while(n>0){
            int a=n%10;
            sum+=a;
            n/=10;
            
        }if(temp%sum==0){
            System.out.println("Harshad Number");
            
        }else{
             System.out.println("Not Harshad Number");
        }
    }
}
