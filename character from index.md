```java
// Java program to get a specific character
// from a given String at a specific index

class Main {

	// Function to get the specific character
	public static char
	getCharFromString(String str, int index)
	{
		return str.charAt(index);
	}

	// Driver code
	public static void main(String[] args)
	{

		// Get the String
		String str = "hello world";

		// Get the index
		int index = 5;

		// Get the specific character
		char ch = getCharFromString(str, index);

		System.out.println("Character from " + str
						+ " at index " + index
						+ " is " + ch);
	}
}
```
