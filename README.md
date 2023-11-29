# Bitvize_calculator
Numeric System Calculator Usage Guide


1 Choose Numeric System:

Enter '2' for binary.
Enter '10' for decimal.
Enter '16' for hexadecimal.

printf("Enter '2' -> binary, '10' -> decimal or '16' -> hexadecimal\n");


2 Calculator Menu:

Choose a bitwise operation:
printf("1. AND, \n2. OR \n3. XOR \n4. NOR \n5. Left Shift \n6. Right shift \n7. Replay \n8. Exit\n");


If an invalid choice is made, it will prompt again.


3 Data Entry:
Enter the numbers based on the chosen numeric system.

For decimal:
char num1[8];
char num2[8];


For binary
char hex1[8];
char hex2[8];

For hexadecimal
char hex1[8];
char hex2[8];

If the entered value is invalid, it will prompt again.

4 Perform Calculation
The selected bitwise operation will be applied to the entered numbers.

printf("The result: %d\n", calculator(dec_dec(num1), dec_dec(num2)));

int a = calculator(bin_dec(bnum1), bin_dec(bnum2));

printf("Hexadecimal: %X\n", calculator(hex_dec(hex1), hex_dec(hex2)));

5 Exiting the Program:
Choose '8' to exit the program.

case 8:
    printf("\tGoodbye\n");
    exit(0);


    Example Usage:

    #include <stdio.h>

int main() {
    int dec = 0;

    printf("Enter '2' -> binary, '10' -> decimal or '16' -> hexadecimal\n");
    do {    
        scanf("%d", &dec);

        if (dec != 10 && dec != 2 && dec != 16) {
            printf("Invalid number system. Please try again\n");
            printf("\t'2' or '10' or '16'\n");
        }
    } while (dec != 10 && dec != 2 && dec != 16);

    determinant(dec);
    return 0;
}

