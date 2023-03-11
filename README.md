# LUG-Assign3

#include <stdio.h>
int main() 
{
  int n, reversed = 0, rem, temp;
    printf("Enter an integer: ");
    scanf("%d", &n);
    temp = n;

    
    while (n != 0) {
        rem = n % 10;
        reversed = reversed * 10 + rem;
        n /= 10;
    }

    
    if (temp == reversed)
        printf("%d is a palindrome.", temp);
    else
        printf("%d is not a palindrome.", temp);

    return 0;
}
