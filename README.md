# java-lab-cse-g-5ef-6c
# EXPERIMENT 6C
## bUILT IN EXCEPTION SCENARIO
source ccode 
```
import java.util.Scanner;

public class Exp6c {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        try {
            System.out.print("Enter divisor for 100: ");
            System.out.println("Result: " + (100 / sc.nextInt()));

            int[] arr = new int[3];
            System.out.println("Accessing index 5... " + arr[5]);

            System.out.print("Enter a string to parse: ");
            System.out.println("Number: " + Integer.parseInt(sc.next()));
        } catch (ArithmeticException e) { System.out.println("ArithmeticException: division by zero.");
        } catch (ArrayIndexOutOfBoundsException e) { System.out.println("ArrayIndexOutOfBoundsException: invalid index.");
        } catch (NumberFormatException e) { System.out.println("NumberFormatException: invalid format.");
        } finally { System.out.println("Program continues..."); }
    }
}



```
# OUTPUT: 
![output of 6c](6c.png)
