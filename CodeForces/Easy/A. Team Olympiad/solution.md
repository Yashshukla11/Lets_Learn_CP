## Here is the solution in Java
````java 
import java.util.ArrayList;
import java.util.Scanner;
 
public class A_Team_Olympiad{
    public static void main(String[] args) {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        int arr[]=new int[n];
        int programming=0,maths=0,pe=0;
        for(int i=0;i<n;i++){
            arr[i]=sc.nextInt();
            if(arr[i]==1)programming++;
            if(arr[i]==2)maths++;
            if(arr[i]==3)pe++;
        }
        ArrayList<Integer> indexP=new ArrayList<>();
        ArrayList<Integer>indexM=new ArrayList<>();
        ArrayList<Integer> indexPE=new ArrayList<>();
        for(int i=0;i<n;i++){
            if(arr[i]==1)indexP.add(i+1);
            if(arr[i]==2)indexM.add(i+1);
            if(arr[i]==3)indexPE.add(i+1);
        }
        if(programming==0||maths==0||pe==0)System.out.println("0");
        else{
            int temp=programming<maths?programming:maths;
            int result=temp<pe?temp:pe;
            System.out.println(result);
        for(int i=0;i<result;i++){
           System.out.println(indexP.get(i)+" "+indexM.get(i)+" "+indexPE.get(i)); 
        }
    }
}
}