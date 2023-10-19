# Student-Grade-Calculator

import java.util.Scanner;

public class studentGradeCalculator {
    public static void main(String[] args) {
        float[] marks = new float[8];
        float sum=0, avg;
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter Marks Obtained in 8 Subjects : ");
        for(int i=0; i<8; i++)
            marks[i] = sc.nextFloat();

        for(int i=0; i<8; i++)
            sum = sum + marks[i];
        avg = sum/8;

        System.out.println();
        System.out.println("Total Marks = "+sum);
        float per = (sum/800)*100;
        System.out.println("Percentage = "+per+"%");
        System.out.print("Grade = ");

        if(avg>=96)
            System.out.println("A+");
        else if(avg>=91 && avg<96)
            System.out.println("A");
        else if(avg>=86 && avg<91)
            System.out.println("B+");
        else if(avg>=81 && avg<86)
            System.out.println("B");
        else if(avg>=76 && avg<81)
            System.out.println("C+");
        else if(avg>=71 && avg<76)
            System.out.println("C");
        else if(avg>=66 && avg<71)
            System.out.println("D+");
        else if(avg>=61 && avg<66)
            System.out.println("D");
        else if(avg>=56 && avg<61)
            System.out.println("E+");
        else if(avg>=51 && avg<56)
            System.out.println("E");
        else if(avg>=46 && avg<51)
            System.out.println("F+");
        else
            System.out.println("F");
    }
}
