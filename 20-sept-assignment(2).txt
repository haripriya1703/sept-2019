#include<stdio.h>
int gcd(int m,int n)
{
    int temp,d;
    if(m<n)
    {
        temp=m;
        m=n;
        n=temp;
    }
    if(m%n==0)
    {
        return n;
    }
    else{
        d=m-n;
        if(d>n)
            return gcd(d,n);
        else
            return gcd(n,d);
    }
}
int main(void)
{

    int a,b,g;
    scanf("%d %d",&a,&b);
    g=gcd(a,b);
    printf("%d",g);
    return 0;
}
