// RamanMishraCodingRound
import java.util.*;
//here we create the class with class_name A
class A{
    //create a fuction name CalculateFactorial where function return value in long data type and passing argument integer type
    public static long calculateFactorial(int n){
        //here we handle base case of recursion for n==0
        if(n==0 ){
            return 1;
        }
        //apply recursion so it call itself untill we reached to result and return the value to function
        return n*calculateFactorial(n-1);
    }
    public static void main(String[] args){
        //take input from user by scanner class 
        Scanner sc=new Scanner(System.in);
        //take variable for user input
        int a=sc.nextInt();
        //checking condition for positive value
        if(a>=0){
            //if input is positive or 0
            System.out.println(calculateFactorial(a));
        }
        else{
            //if input is negative
            System.out.println("Please Enter A positive no ");
        }
    }
}
