#include<stdio.h>
#include<string.h>
int main(void)
{
    char s[100],temp,i,j;
    scanf("%s",s);
    for(i=0,j=strlen(s)-1;i<j;i++,j--)
    {
        if(s[i]=='a' ||s[i]=='e' ||s[i]=='i' ||
           s[i]=='o' ||s[i]=='u' ||s[i]=='A' ||
           s[i]=='E' ||s[i]=='I' ||s[i]=='O' ||s[i]=='U')
        {
            i++;
        }
        if(s[i]=='a' ||s[i]=='e' ||s[i]=='i' ||
           s[i]=='o' ||s[i]=='u' ||s[i]=='A' ||
           s[i]=='E' ||s[i]=='I' ||s[i]=='O' ||s[i]=='U')
           j--;
        temp=s[i];
        s[i]=s[j];
        s[j]=temp;

    }
    printf("%s",s);
    return 0;
}
