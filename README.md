# calculator
import java.util.*;

class Calculator 
{

      public static void main(String[] args) {
      
               double num1, num2, ans;
               char ch;

      Scanner scn = new Scanner(System.in);
      
      System.out.print("Enter two numbers: ");
      num1 = scn.nextDouble();
      num2 = scn.nextDouble();

      System.out.print("\n Enter an operator (+, -, *, /) : ");
      ch = scn.next().charAt(0);

      switch(ch) {
         case '+' : ans = num1 + num2;
            break;
         case '-' : ans = num1 - num2;
            break;
         case '*' : ans = num1 * num2;
            break;
         case '/' : ans = num1 / num2;
            break;
      default : System.out.print("Error! Enter correct operator");
         return;
      }
      
      System.out.print("\n The result is given as follows: \n");
      System.out.printf(num1 + " " +  ch + " " + num2 + " = " + ans);
   }
}
