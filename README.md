#include<stdio.h>

unsigned long long factorialiterative(int n);
unsigned long long factorialrecursive(int n);

int main(){
int num:
printf("enter a number");
scanf("%d",&num);

if(num<0){
printf("factorial is not defined for negative numbers.\n");
}

else{ printf("iterative;%d!=%llu\n",num,factorialiterative(num));
  printf("recursive;%d!=%llu\n",num,factorialrecursive(num));

}
  return 0;

  }
    unsigned long long factorialiterative(int n)
    {
    unsigned long long res =1;
    for(int i=2;i<=n;i++)res*=i;

      return res;
      }
      unsigned lonf long factorialrecursive(int n)
      {
      if(n<=1) return 1;
      return n * factorialrecursive(n-1);
      }


