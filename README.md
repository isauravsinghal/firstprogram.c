#include <stdio.h>

int main()
{
Label:

    printf("Which conversion do you want:\n    1) kms to miles\n    2) inches to foot\n    3) cms to inches\n    4) pounds to kgs\n    5) inches to meters\n");
    int n,x;
    float  first,second;
    

    printf("Enter the input character:");
    scanf("%d", &n);

    switch (n)
    {
    case 1:
        printf("Enter the quantity in Kms:");
        scanf("%f", &first);
        second = first * 0.621371;
        printf("%.2f kms is approximately equals to %0.2f miles\n", first, second);

        break;
    case 2:
        printf("Enter the quantity in inches:");
        scanf("%f", &first);
        printf("%.2f inches is approximately equals to %0.2f foots\n", first, first * 0.0833333);
        break;
    case 3:
        printf("Enter the quantity in cms:");
        scanf("%f", &first);
        printf("%.2f cms is approximately equals to %0.2f inches\n", first, first * 0.393701);
        break;
    case 4:
        printf("Enter the quantity in pounds:");
        scanf("%f", &first);
        printf("%.2f pounds is approximately equals to %0.2f kgs\n", first, first * 0.453592);
        break;
    case 5:
        printf("Enter the quantity in inches:");
        scanf("%f", &first);
        printf("%.2f inches is approximately equals to %0.2f meters\n", first, first * 0.0254);
        break;

    default:
    {
        printf("Only input 1,2,3,4 or 5 for the converversions\n");
        goto Label;
    }
    }

    printf("Thankyou for coming\n");
    printf("Enter any number to exit:");
    scanf("%d", x);
    return 0;
}
