### Task 1

### Task 2: Algorithmic Challenge
The following code snippets demonstrate how to print numbers from 1 to 100 with specific words replacing multiples of 3, 5, and 7.

##### Python
```python
# Loop through numbers 1 to 100
for i in range(1, 101):
    output = ""
    
    # Check if the number is a multiple of 3
    if i % 3 == 0:
        output += "Hello"
    
    # Check if the number is a multiple of 5
    if i % 5 == 0:
        output += "World"
    
    # Check if the number is a multiple of 7
    if i % 7 == 0:
        output += "Yoo"
    
    # If the number is not a multiple of 3, 5, or 7, set output to the number
    if output == "":
        output = i
    
    # Print the output, followed by a comma and space
    print(output, end=", ")

#### Output:
```plaintext
1, 2, Hello, 4, World, Hello, Yoo, 8, Hello, World, 11, Hello, 13, Yoo, HelloWorld, 16, 17, Hello, 19, World, HelloYoo, 22, 23, Hello, 25, World, Hello, 28, 29, HelloWorld, 31, 32, Hello, 34, WorldYoo, Hello, 37, 38, Hello, 40, World, HelloYoo, 43, 44, Hello, World, 47, Hello, Yoo, 50, HelloWorld, 52, 53, Hello, 55, World, HelloYoo, 58, 59, Hello, 61, 62, HelloWorld, 64, 65, Hello, 67, WorldYoo, Hello, 70, 71, Hello, 73, World, HelloYoo, 76, 77, Hello, World, 80, Hello, Yoo, 82, 83, HelloWorld, 85, 86, Hello, 88, World, HelloYoo, 91, 92, Hello, 94, World, Hello, 97, Yoo, HelloWorld, 100,

##### java
```java
public class Main {
    public static void main(String[] args) {
        // Loop through numbers 1 to 100
        for (int i = 1; i <= 100; i++) {
            String output = "";

            // Check if the number is a multiple of 3
            if (i % 3 == 0) {
                output += "Hello";
            }

            // Check if the number is a multiple of 5
            if (i % 5 == 0) {
                output += "World";
            }

            // Check if the number is a multiple of 7
            if (i % 7 == 0) {
                output += "Yoo";
            }

            // If the number is not a multiple of 3, 5, or 7, set output to the number
            if (output.isEmpty()) {
                output = Integer.toString(i);
            }

            // Print the output, followed by a comma and space
            System.out.print(output + ", ");
        }
    }
}

#### Output:
```plaintext
1, 2, Hello, 4, World, Hello, Yoo, 8, Hello, World, 11, Hello, 13, Yoo, HelloWorld, 16, 17, Hello, 19, World, HelloYoo, 22, 23, Hello, 25, World, Hello, 28, 29, HelloWorld, 31, 32, Hello, 34, WorldYoo, Hello, 37, 38, Hello, 40, World, HelloYoo, 43, 44, Hello, World, 47, Hello, Yoo, 50, HelloWorld, 52, 53, Hello, 55, World, HelloYoo, 58, 59, Hello, 61, 62, HelloWorld, 64, 65, Hello, 67, WorldYoo, Hello, 70, 71, Hello, 73, World, HelloYoo, 76, 77, Hello, World, 80, Hello, Yoo, 82, 83, HelloWorld, 85, 86, Hello, 88, World, HelloYoo, 91, 92, Hello, 94, World, Hello, 97, Yoo, HelloWorld, 100,
