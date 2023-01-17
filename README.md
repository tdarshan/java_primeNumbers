# java_primeNumbers

// code : 

import java.util.Scanner;

public class HelloWorld {
    public static void main(String[] args) {
        
        Scanner sc = new Scanner(System.in);
        
        System.out.println("Enter a number for range : ");
        int t = sc.nextInt();
        
        for(int i = 1; i<= t; i++){
          int count = 0;
          
          for(int div = 2; div*div <= i; div++){
            if(i%div == 0){
              count += 1;
              break;
            }
          }
          
          if(count == 0){
            System.out.println(i + " is Prime");
          }
          else{
            System.out.println(i + " is not-Prime");
          }
        }
    }
}
