# C_refreshment



// Online C compiler to run C program online
#include <stdio.h>

int main() {
    int num1, num2;
    printf("enter any two numbers\n");
    scanf("%d%d",&num1 , &num2);
    if(num1>num2)
    printf("num1 is greater then num2");
    else
    printf("num2 is greater than num1");

    return 0;
}







// Online C compiler to run C program online
#include <stdio.h>

int main() {
int i,j,k,l=7;
for(i=1;i<l;i++)
    {
        for(j=1;j<=l-i;j++)
        {
            printf(" ");
        }
    for(k=i;k<=2*i-1;k++)
            {
                printf("*");
            }
            printf("\n");
        
    }
    
    return 0;
}






//C program  for square a numberr using function
#include <stdio.h>
 
int sq(int x);

int main() {
    int  m,result,x;
    
    m = sq(x);
    printf("%d",m);
    return 0;
}
int sq(int x)
{
    scanf("%d",&x);
   int result=0;
     result = x*x ;
    return result;
}







// farenheight to celcius conversion using function
#include <stdio.h>
int conv(int far);
int main() {
    //  C is celcius value for input farenheit value
    int C,far;
    C= conv(far);
    printf("%d",C);
    return 0;
}
int conv(int far)
{
    int degC;
    
    scanf("%d",&far);
    degC = (far-32)*5/9;
    return degC;
}







// check given number is odd or even using function
#include <stdio.h>
int check(int x);
int main() {
int y,x;
    y=check(x);
    printf("%d",y);

    return 0;
}
int check(int x)
{
    scanf("%d", &x);
    if(x%2 == 0)
    return 1;
    else
    return 0;
}






//C program  for square and cube of a number using function
#include <stdio.h>
int sq(int x);
int cube(int x);

int main() {
    int  m,x,n;
    scanf("%d",&x);
    
    m = sq(x);
    n= cube(x);
    printf("square of given number is %d\n",m);
    printf("cube of a given number is %d",n);
    return 0;
}
int sq(int x)
{
   int result=0;
     result = x*x ;
    return result;
}
int cube(int x)
{
    int z=0;
    z = x *x *x;
    return z;
}






//C program  for swap 2 numbers using pointer
#include <stdio.h>

int swap(int *m, int *n);
int main() {
    int m,n;
    scanf("%d",&m);
    scanf("%d",&n);
    
    printf("before swap:\n");
    
    printf("num1 is %d\n",m);
    printf("num2 is %d\n",n);
    
    printf("after swap:\n");
    
    swap(&m,&n);
    printf("num1 is %d\n num2 is %d", m,n);
    //printf("num2 is %d\n",n);
    return 0;
}
int swap(int *m, int *n)
{
   
    int o=*m;
    *m=*n;
    *n=o;
    return ;
}









//C program  for swap 2 numbers using function
#include <stdio.h>

int swap(int m, int n);

    
int main() {
    int m,n;
    scanf("%d",&m);
    scanf("%d",&n);
    printf("before swap:\n");
    
    printf("num1 is %d\n",m);
    printf("num2 is %d\n",n);
    
    printf("after swap:\n");
    
    swap(m,n);
    
    return 0;
}
int swap(int m, int n)
{
   
    int o=m;
    m=n;
    n=o;
    printf("num1 is %d\n num2 is %d",m,n);
}







// program for find the sum  and product of two numbers using pointers
#include <stdio.h>
int sumpro(int *x,int*y);
int sum,pro;
int main() {
    int x,y;
    scanf(" %d",&x);
    scanf(" %d",&y);
    sumpro(&x,&y);

    return 0;
}
int sumpro(int *x,int *y)
{
    sum = *x+*y;
    pro = *x**y;
    printf("sum of two number is: %d product of two nnumber is: %d",sum,pro);
}









// average of array numbers using function
#include <stdio.h>
int size;
float average(int array[], int size);
int main() {
    int i;
    printf("Enter the size :");
    scanf("%d",&size);
 printf("Enter the array elements :");
 int array[size];
    for (i=0;i<size;i++)
    {
    scanf("%d",&array[i]);
    }
       average(array,size);
    return 0;
}
float average(int array[],int size)
{
   int sum , i;
   float avg;
   for(i=0;i<size;i+)
   {
       sum = sum+ array[i];
   }
 avg = sum/size;
       printf("average is %f",avg);
}


