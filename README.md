# zoho-recruitment-2020
#include<stdio.h>
void main()
{
    char a[20];
    int i,j,n,c;
    clrscr();
    printf("enter the string:");
    gets(a);
    n=strlen(a);
    c=n/2;
    for(i=0;i<n;i++)
    {
    for(j=n-1;j>i;j--)
    {
       printf("  ");
        }
    for(j=c;j<=c+i&&j<n;j++)
    {
       printf("%c",a[j]);
    }
    if(i>c)
    {
           for(j=0;j<i-c;j++)
       {
           printf("%c",a[j]);
       }
        }
    printf("\n");
    }
    getch();
}
