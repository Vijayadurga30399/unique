# unique#
include <stdio.h>
#include <string.h>
#include <math.h>
#include <stdlib.h>
int main() {
    int i,j,n,t,c=0,flag=0,p=0,k,f[26]={0},a,b,r;
    scanf("%d",&n);
    for(i=0;i<n;i++)
    {c=0; 
     flag=0;
    scanf("%d %d",&a,&b);
       for(j=a;j<=b;j++)
        { 
           t=j;
           while(t>0)
           {
               r=t%10;
               f[r]++;
               t=t/10;
           }
         for(k=0;k<10;k++)
         {
             if(f[k]<=1){
             flag=0;
                }
             //printf("%d %d",f[k],a);}
             else{
                 flag=1;
             break;}
         }
           if(flag==0)
         {
             ++c;
         }
         
       for(k=0;k<10;k++)
           f[k]=0;
       }
       printf("%d\n",c);
    }
            
         return 0;
}
