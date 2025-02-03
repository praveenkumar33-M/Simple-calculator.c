# Simple-calculator.c
Praveen kumarL14 

#include <stdio.h>

int main() {
    int choice;
    float num1, num2;

    // Displaying the menu
    printf("Simple Calculator\n");
    printf("==================\n");
    printf("1. Addition\n");
    printf("2. Subtraction\n");
    printf("3. Multiplication\n");
    printf("4. Division\n");
    printf("Enter your choice (1/2/3/4): ");
    scanf("%d", &choice);

    // Taking input for numbers
    printf("Enter two numbers: ");
    scanf("%f %f", &num1, &num2);

    // Perform the operation based on user's choice
    switch(choice) {
        case 1:
       printf("Result: %.2f\n", num1 + num2);
            break;
        case 2:
       printf("Result: %.2f\n", num1 - num2);
            break;
        case 3:
      printf("Result: %.2f\n", num1 * num2);
            break;
        case 4:
            if (num2 != 0) {
       printf("Result: %.2f\n", num1 / num2);
            } 
         else {
         printf("Error! Division by zero.\n");
            }
           break;
        default:
            printf("Invalid choice! Please choose between 1 and 4.\n");
    }

    return 0;
}
