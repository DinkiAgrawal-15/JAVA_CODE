```java
public class AreaOfTrapizoid {
 
    public static void main(String[] args) {
        double side1, side2, height, area;
        Scanner scanner;
        scanner = new Scanner(System.in);
 
        // Take input from user
        System.out.println("Enter Length of Two Parallel Sides of Trapezium");
        side1 = scanner.nextDouble();
        side2 = scanner.nextDouble();
        System.out.println("Enter Height of Trapezium");
        height = scanner.nextDouble();
 
        /*
         * Area of trapezium = ((Sum of parallel sides)*height)/2 = 1/2 X
         * (parallelSideOne + parallelSideTwo) X height)
         */
 
        area = 1.0 / 2 * (side1 + side2) * height;
 
        System.out.format("Area of Trapezium = %.2f\n", area);
    }
}
```
