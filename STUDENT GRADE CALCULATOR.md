
import java.util.Scanner;

public class StudentGradeCalkulator
{

    public static void main(String[] args)

    {
        Scanner scanner = new Scanner(System.in);

        System.out.print("Enter number of Subjects= ");
        int numSub = scanner.nextInt();

        int Tmarks =0;
        for(int i = 1; i <= numSub ; i++)
        {
            System.out.println("Enter the marks obtained in sub"+ i +":");
            int marks = scanner.nextInt();
            Tmarks += marks ;

        }

        float avgPertg = (float) Tmarks / numSub ;

        String Grade ;

        if(avgPertg >= 85)
        {
            Grade ="AA";
        }

        else if(avgPertg >=75)
        {
            Grade = "A";
        } else if (avgPertg >=60)
        {
            Grade = "B";
        }else if (avgPertg >=50)
        {
            Grade = "C";
        }else if (avgPertg >=40)
        {
            Grade = "D";
        }else if (avgPertg >=35)
        {
            Grade = "E";
        }

        else

        {
            Grade = "F";
        }


        System.out.println("Total Marks :"+ Tmarks );
        System.out.println("Average Percentage :"+ avgPertg);
        System.out.println("Grade : "+ Grade);

        scanner.close();
    }

}
