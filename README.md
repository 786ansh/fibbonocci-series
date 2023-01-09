# fibbonocci-series
#include <stdio.h>
int fibbo(int);


int main()
{
    int n;
    printf("enter no of terms:");
    scanf("%d",&n);
    fibbo(n);

    return 0;
}
int fibbo(int n)
{
    int a=-1,b=1,c;
    for(int i=1;i<=n;i++)
    {
        c=a+b;
        printf("%d\n",c);
        a=b;
        b=c;
    }
}

