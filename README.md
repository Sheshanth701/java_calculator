# java_calculator
import java.util.Scanner;
public class Calculator{
public static void main(String[] args){

Scanner scanner = new Scanner(system.in);
System.out.println("enter first character");
double num1=scanner.nextDouble();
System.out.println("enter the operation to be performed( +,-,*,/)");
char operator=scanner.next().charAt(0);
System.out.println("enter the second character");
double num2=scanner.nextDouble();
double result;
switch(operator){
  case'+':
  result=num1+num2;
  break;
  case'-':
  result=num1-num2;
  break;
  case'*':
  result=num1*num2;
  break;
  case'/':
  if(num2!=0){
  result=num1/num2;
  }else{
  System.out.println("error 404! division by 0 ");
  return;
  }
  break;
  default:
  System.out.println("invalid operation");
  return;
  }
System.out.println("the result is "+result);
}
}
  
  
