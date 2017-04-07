# fibonacci

package fibonacci;
import java.util.Scanner;

public class Fibonacci {
    
    private static Scanner scanner = new Scanner (System.in);

    public static void main(String[] args) {
        
        System.out.print("Input : ");
        int input = scanner.nextInt();
        int fib = 1;
        System.out.print ("1 1 ");
        
        int temp;
        int fib2 = 1;
        for(int i = 2 ; i<input; i++){
            temp = fib + fib2;
            System.out.print(temp + " ");
            fib = fib2;
            fib2 = temp;
        }
    
    }
    
}
