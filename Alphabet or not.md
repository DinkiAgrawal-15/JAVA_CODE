```java
import java.util.Scanner;

public class Main
{
	public static void main(String[] args) {
	    char ch;
	    Scanner sc= new Scanner(System.in);
	    
	    
	    ch=sc.next().charAt(0);
	    if((ch>='a'&& ch<='z')|| (ch>='A'&& ch<='Z')){
	    
	    
	        		System.out.printf("Alphabet");
				

	    }else{
	        		System.out.printf("Not Albhabet");

	    }
	}
	
}
```
