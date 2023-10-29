## Here is the solution in Java
````java 
import java.util.Scanner;
 
public class B_Borze{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        String str=sc.nextLine();
        StringBuilder sb=new StringBuilder();
        for(int i=0;i<str.length();i++){
        if(str.charAt(i)=='.'){
            sb.append("0");
        }
        else if(str.charAt(i)=='-'&&str.charAt(i+1)=='.'){
            sb.append("1");
            i++;
        }
        else if(str.charAt(i)=='-'&&str.charAt(i+1)=='-'){
            sb.append("2");
            i++;
        }
    }
    sc.close();
    System.out.println(sb);
}
}