#include<stdio.h>
#include<string.h>
int main(void)
{
int a[256]={0},i,j;
char s[100];
scanf("%s",s);
for(i=0;i<strlen(s);i++)
{
a[(int)s[i]]++;
}
for(j=0;j<256;j++)
{
if(a[j]!=0)
    {
printf("%c-%d\n",(char)j,a[j]);
}
}
return 0;
}
