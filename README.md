# list-of-all-prime-numbers-of-a-given-range-and-no-of-prime-no-in-range
in java



import java.util.*;
import java.io.*;
public class HelloWorld{

    public static void main(String []args)
    {
        Scanner sc=new Scanner(System.in);
        int n=sc.nextInt();
        
        System.out.println(check(n));
    }
    static int check(int n)
    {
        
        int p=0,count=0;
        List<Integer> li=new ArrayList<>();
        for(int i=1;i<=n;i++)
        {
            count=0;
            for(int j=2;j<i;j++)
            {
                if(i%j==0 )
                {
                    count++;
                    break;
                }
                
            }
            if(count==0 )
                {
                li.add(i);
                System.out.println(li.get(p));
                p++;
                
                }
            
            
        }
        return li.size();
    } 
    
}
