# java-part-3


import java.util.Scanner;

public class Main {
    public static void main(String[] args) {

        // Example 1: Print "Java is awesome" multiple times
        int a = 5;
        for (int i = 1; i <= a; i++) {
            System.out.println("Java is awesome");
        }

        // Example 2: Print numbers from 1 to 10
        for (int i = 1; i <= 10; i++) {
            System.out.println(i);
        }

        // Example 3: Print numbers from 10 to 1 (reverse order)
        for (int i = 10; i >= 1; i--) {
            System.out.println(i);
        }

        // Example 4: Sum of first n natural numbers (1 to 1000)
        int sum = 0;
        int x = 1000;
        for (int i = 1; i <= x; i++) {
            sum += i;  // Equivalent to sum = sum + i
        }
        System.out.println("Sum of natural numbers = " + sum);

        // Example 5: For-each loop (array iteration)
        int[] numbers = {3, 7, 5, -5};
        for (int number : numbers) {
            System.out.println(number);
        }

        // Example 6: Sum of array elements
        int[] array = {3, 4, 5, -5, 0, 12};
        sum = 0;
        for (int num : array) {
            sum += num;
        }
        System.out.println("Sum of the array = " + sum);

        // Example 7: Display vowels using a for loop
        char[] vowels = {'a', 'e', 'i', 'o', 'u'};
        for (char vowel : vowels) {
            System.out.println(vowel);
        }

        // Example 8: Print 1 to 5 using a while loop
        int i = 1;
        while (i <= 5) {
            System.out.println(i);
            i++;
        }

        // Example 9: Sum of positive numbers using a while loop
        sum = 0;
        Scanner input = new Scanner(System.in);

        System.out.println("Enter a number: ");
        int number = input.nextInt();

        while (number > 0) {
            sum += number;
            System.out.println("Enter a number: ");
            number = input.nextInt();
        }
        System.out.println("Sum of positive numbers = " + sum);
        input.close();

        // Example 10: Print 1 to 5 using a do-while loop
        i = 1;
        int n = 5;
        do {
            System.out.println(i);
            i++;
        } while (i <= n);

        // Example 11: Break statement example
        for (i = 1; i <= 10; i++) {
            if (i == 5) {
                break;
            }
            System.out.println(i);
        }

        // Example 12: Continue statement example
        for (i = 1; i <= 10; i++) {
            if (i > 4 && i < 9) {
                continue;
            }
            System.out.println(i);
        }

        // Example 13: Switch statement example
        number = 48;
        String size;
        switch (number) {
            case 29:
                size = "small";
                break;
            case 42:
                size = "medium";
                break;
            case 44:
                size = "large";
                break;
            case 48:
                size = "extra large";
                break;
            default:
                size = "unknown";
                break;
        }
        System.out.println("Size: " + size);
    }
}
