#include<stdio.h>
int main()
{
    int r, n, b=0, base=1;
    printf("Enter the Number in Decimal Form\n");
    scanf("%d",&n);
    for(;n>0;)
    {
        r=n%2;
        b=b+r*base;
        n=n/2;
        base=base*10;
    }
    printf("Binary number is %d",b);
    return 0;
}
