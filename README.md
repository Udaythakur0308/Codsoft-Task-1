# Codsoft-Task-1
//Task-1 Student Grade Calculator:-
import java.util.*;
class Stu_Grade_Cal{
    public static void main(String args[]){
        Scanner sc=new Scanner(System.in);
        System.out.println("Enter Number of Subjects : ");
        int ns=sc.nextInt();
        int total=0;
        for(int i=1;i<=ns;i++) {
            System.out.println("Enter marks obtained in  :" + i + " : ");
            int marks = sc.nextInt();
            total += marks;
        }
        double averP=(double)total/ns;
        char Grade;
        if(averP>=90){
            Grade='A';
        }
        else if(averP>=80){
            Grade='B';
        }
        else if(averP>=70){
            Grade='C';
        }
        else if(averP>=60){
            Grade='D';
        }
        else if(averP>=50){
            Grade='E';
        }
        else{
            Grade='F';
        }
        System.out.println("Total marks score is : "+total);
        System.out.println("Average Percentage gained is  : "+averP+"%");
        System.out.println("Grade : "+Grade);


    }
}
