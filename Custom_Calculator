package sakshimbheda;

import java.util.Scanner;

class InvalidInput extends Exception{
    @Override
    public String toString(){
        return "Operator is invalid";
    }
}
class MaxInputException extends Exception{
    @Override
    public String toString(){
        return "Input can't be greater than 1 lakh";
    }
}
class MaxMultiplierException extends Exception{
    @Override
    public String toString() {
        return "Input can't be greater than 7 thousand in multiplication";
    }
}
public class Customcal extends Exception{


    public static void operatorCheck(String opr) throws InvalidInput {
        if (opr.equals("+") || opr.equals("-") || opr.equals("*") || opr.equals("/")) return;
        throw new InvalidInput();
    }
    public static double add(int x,int y) throws MaxInputException {
        if (x>100000||y>100000) throw new MaxInputException();
        System.out.println("The value of "+x+" + "+y+" is : ");
        return x+y;
    }
    public static double subtract(int x,int y) throws MaxInputException {
        if (x>100000||y>100000) throw new MaxInputException();
        System.out.println("The value of "+x+" - "+y+" is : ");
        return x-y;
    }
    public static double multiply(int x,int y) throws MaxMultiplierException {
        if (x>7000||y>7000) throw new MaxMultiplierException();
        System.out.println("The value of "+x+" * "+y+" is : ");
        return x*y;
    }
    public static double divide(int x,int y) throws MaxInputException,ArithmeticException {
        if (x>100000||y>100000) throw new MaxInputException();
        System.out.println("The value of "+x+" / "+y+" is : ");
        return x/y;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the operator(only +,-,*,/ are allowed): ");
        String opr = sc.next();
        try {
            operatorCheck(opr);
        }
        catch (Exception e){
            System.out.println(e);
            return;
        }
        System.out.println("Enter the first number : ");
        int x = sc.nextInt();
        System.out.println("Enter the second number : ");
        int y = sc.nextInt();
        if (opr.equals("+")){
            try{
                System.out.println(add(x,y));
            }
            catch (Exception e){
                System.out.println(e);
            }
        }
        else if (opr.equals("-")){
            try{
                System.out.println(subtract(x,y));
            }
            catch (Exception e){
                System.out.println(e);
            }
        }
        else if (opr.equals("*")){
            try{
                System.out.println(multiply(x,y));
            }
            catch (Exception e){
                System.out.println(e);
            }
        }
        else {
            try{
                System.out.println(divide(x,y));
            }
            catch (Exception e){
                System.out.println(e);
            }
        }

    }
}
