#include<stdio.h>
int main(void)
{
    int a,b,i,j,max=0;
    scanf("%d %d",&a,&b);
    if(a<=b)
    {
        for(i=1;i<=a;i++)
        {
            if(a%i==0 && b%i==0)
                max=i;
        }

    }
    else
    {
        for(i=1;i<=b;i++)
        {
            if(a%i==0 && b%i==0)
                max=i;
        }
    }
    printf("%d",max);
    return 0;
}
