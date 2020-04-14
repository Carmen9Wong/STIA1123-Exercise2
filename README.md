# STIA1123-Exercise2Q1
package com.company;
public class Square {
public static void main(String[]args){
System.out.println("Number "+"\t\t"+"Square"+"\t\t"+"Cube");
for(int i=0;i<=10;i++){
System.out.println( i+" \t\t"+ (int)Math.pow(i,2) + " \t\t"+(int)Math.pow(i,3));
        }
    }
}

Q2
package com.company;
import java.util.Scanner;
public class A{
public static void main(String[]args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter a string ：");
String a = sc.nextLine();
int sum =0;
for(int i=0;i<a.length();i++){
if (a.charAt(i)=='A'){
sum++;
}
}
System.out.println("The num of times the character'A' is found : "+sum);
}
}

Q3
package com.company;
import java.util.Scanner;
public class PrintReverse{
public static void main(String[]args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter a string ：");
String o = sc.nextLine();
String total = " ";
    for(int i=o.length()-1;i>=0;i--){
        total+=o.charAt(i);
    }
    System.out.println("Reverse string is : "+total);
}
}

Q4
package com.company;
import java.util.Random;
import java.util.Scanner;
public class RandomInRange {
public static void main(String[]args){
Scanner sc = new Scanner(System.in);
System.out.println("Enter integer 10：");
int min = sc.nextInt();
System.out.println("Enter integer 20：");
int max = sc.nextInt();
        if(min>max){
            System.out.println("integer 10 is greater than integer 20 = 00");
        }else{
            System.out.println("integer 20 is greater than integer 10");
            random(min,max);
        }
    }

    public static void random(int min,int max){
        Random in = new Random();
        int range = max-min+1;
        System.out.println("Random integer : "+in.nextInt(range));

        //system.out.println((int)(Math.random()*(max-min+1))+low);
    }
}
