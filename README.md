#include<stdio.h>
void interchange(int * u,int *v);
int main(void)
{
   int x=5,y=10;
   printf("Originally x=%d and y=%d\n",x,y);
   interchange(&x,&y); //需要记住，这里输入的是值的地址，！！不是别的。 
   printf("Now, x=%d and y=%d \n",x,y);
   return 0;
}
void interchange(int *u,int *v)
{
    int temp;
    temp=*u;
    *u=*v;
    *v=temp;
}
