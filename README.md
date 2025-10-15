 #include <stdio.h>

    int main() {

    printf("Jhon Mark Navales Elaydo\n");
    printf("2025303548\n");

    int x, y;
    char operator; 
    int result;    

    printf("Enter 1st Number: ");
    scanf("%d", &x);

    printf("Enter 2nd Number: ");
    scanf("%d", &y);

    printf("Enter An Operator (+, -, *, /, %%): ");
    scanf(" %c", &operator);  

    switch(operator) {
        case '+':
            result = x + y;
            printf("Result of %d + %d is %d\n", x, y, result);
            break;

        case '-':
            result = x - y;
            printf("Result of %d - %d is %d\n", x, y, result);
            break;

        case '*':
            result = x * y;
            printf("Result of %d * %d is %d\n", x, y, result);
            break;

        case '/':
            if (y != 0) {
                result = x / y;  
                printf("Result of %d / %d is %d\n", x, y, result);
            } else {
                printf("Error: Division by zero is not allowed\n");
            }
            break;

        case '%':
            if (y != 0) {
                result = x % y;
                printf("Result of %d %% %d is %d\n", x, y, result); 
            } else {
                printf("Error: Modulo by zero is not allowed\n");
            }
            break;

        default:
           
            printf("Invalid operator. Please use +, -, *, /, or %%\n");
            break;
    }

    return 0;

}
