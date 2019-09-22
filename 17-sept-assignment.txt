#include<stdio.h>
#include<string.h>
int main(void)
{
int a[256]={0},b[256]={0},f=0,i,j;
char r[100],s[100];
scanf("%s",s);
scanf("%s",r);
for(i=0;i<strlen(s);i++)
{
a[(int)s[i]]++;
b[(int)r[i]]++;
}
for(j=0;j<256;j++)
{
if(a[j]!=b[j])
{
f=-1;
break;
}
}
if(f==-1)
{
printf("the given strings are not anagrams");
}
else
{
printf("the given strings are anagrams");
}
return 0;
}
