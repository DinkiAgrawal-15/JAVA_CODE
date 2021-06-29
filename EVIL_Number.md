```java
import java.util.*;
public class Main {  
  
    //main() method start  
    public static void main(String args[])  
    {  
        int range;  
          
        //create scanner class object  
        Scanner sc=new Scanner(System.in);  
          
        //show custom message  
        System.out.println("Enter the value of range");  
          
        //store user entered value into variable range  
        range = sc.nextInt();  
  
        for(int i = 1; i <= range; i++)  
            if(checkNumber(i)){  
                System.out.println(i + " is an Evil number");  
            }  
    }  
      
    // create checkNumber() method that returns true when it founds number Evil   
    public static boolean checkNumber(int n) {  
  
        // find the equivalence binary number using user defined convertToBinary() method  
        long binaryNumber = convertToBinary(n);  
  
        // find total number of 1's in binary number  
        int count = 0;  
  
        // iterate each digit of binary number  
        while(binaryNumber != 0) {  
  
            // if the last digit of binary number is 1, increase the count value  
            if(binaryNumber % 10 == 1)   
                count++;  
  
            // remove the last digit from the number  
            binaryNumber = binaryNumber / 10;  
        }  
  
        // check whether the value of count is even or odd  
        if(count % 2 == 0)  
            return true;    //return true when the value of count is even  
  
        //return false if the value of the count is false  
        return false;  
    }  
  
    //create convertToBinary() method to convert the decimal value into binary  
    private static long convertToBinary(int number) {  
        long binaryNumber = 0;  
        int rem = 0;  
        int j = 1;  
        while(number != 0) {  
            rem = number % 2;  
            binaryNumber += rem * j;  
            number = number / 2;  
            j = j * 10;  
        }  
          
        return binaryNumber;    //return the binary equivalent number of the decimal number  
    }  
}
```
