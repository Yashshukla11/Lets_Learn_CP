## Here is the solution in Java
````java 
import java.util.ArrayList;
import java.util.Scanner;
 
public class A_Short_Substrings{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        sc.nextLine();
        while(n>0){
            String str=sc.nextLine();
            StringBuilder sb=new StringBuilder();
            for(int i=0;i<str.length()-1;i+=2){
                sb.append(str.substring(i, i+1));
            }
            sb.append(str.substring(str.length()-1));
            System.out.println(sb);
            n--;
        }
    }
}