#include<stdio.h>
void read(int a[],int n)
{
   for(int i=0;i<n;i++)
   {
     scanf("%d",&a[i]);
   }
}
void swap(int*a,int *b)
{
    int temp;
    temp=*a;
    *a=*b;
     *b=temp;
}
void sort(int a[],int n )
{
   int i,j,min;
   for(i=0;i<n-1;i++)
   {
   min=i;
   for(j=i+1;j<n;j++)
   { 
      if(a[j]<a[min])
      {
      min=j;
      }
      if(min!=i)
      
      swap(&a[i],&a[min]);
      
   }
   }
}
void print(int a[],int n)
{ 
   for(int i=0;i<n;i++)
   {
      printf(" %d",a[i]);
   }
}
int main()
{ 
int a[100],n;
printf("enter the no.of .elements in array");
scanf("%d",&n);
printf("enter %d elements",n);
read(a,n);
sort(a,n);
print(a,n);
}
