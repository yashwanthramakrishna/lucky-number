# lucky-number
import java.util.*;

 // Compiler version JDK 11.0.2

 class Dcoder
 {
   public static void main(String args[])
   { 
     int num, digit,sum=0,count;
   Scanner in=new Scanner(System.in);
    System.out.println("enter car number!");
    num=in.nextInt();
     count=0;
     while ( num!=0 )
     {
       digit=num%10;
       sum=sum+digit;
      num= num/10;
       count++;
       
       
     }
     
     if(count==4)
     {
       if((sum%3==0)||(sum%5==0)||(sum%7==0))
       {
         System.out.println("lucky number");
       }
       else
          {
         System.out.println("not a lucky number");
          }
          
     }
    else{
      System.out.println("it is not a valid number");
       }
   }
 }
