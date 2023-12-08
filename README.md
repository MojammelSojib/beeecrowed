check prime number
#include<stdio.h>
int main()
{
    int n,count=0,totalprime=0,sum=0;

    for(n=1;n<=10000;n++){
            count=0;
    if(n<=1){
            count=1;
        }
        else{
        for(int i=2;i<n;i++){
            if(n%i==0){
                count++;
                break;
            }
         }
        }
        if(count==0)
        {
            printf("%d \n",n);
    totalprime++;
    sum=sum+n;
         }
        }
        printf("Total Prime Numbers:%d \n",totalprime);
        printf("Total Sum Prime Numbers:%d ",sum);
        return 0;

}
check factorial number code

#include<stdio.h>
int main()
{
  int i,fact=1,n;
  printf("Enter any positive number:");
  scanf("%d",&n);

  for(i=1;i<=n;i++)
  {
      fact =fact*i;
  }
  printf("%d\n",fact);
  return 0;
}

**sum of digits**
#include<stdio.h>
int main()
{
    int num,tem,r,sum=0;
    printf("Enter any number ");
    scanf("%d",&num);

    tem=num;
    while(tem!=0)
    {
        r=tem%10;
        sum=sum+r;
        tem=tem/10;
    }
    printf("%d",sum);

}

**revers of number**

#include<stdio.h>
int main()
{
    int n,tem,r,sum=0;
    printf("Enter your number ");
    scanf("%d",&n);

    tem=n;

      while (tem!=0) {
        r = tem % 10;
        sum = sum * 10 + r;
        tem = tem / 10;
    }
  printf("Revers of number %d",sum);
    return 0;
}


**Palindrome number**


#include<stdio.h>
int main()
{
    int n,tem,r,sum=0;
    //printf("Enter any number ");
    scanf("%d",&n);

    tem=n;
    while(n!=0)
    {
        r=tem%10;
        n=sum*10+r;
        tem=tem/10;
    }
    if(n==sum){
        printf("Palindrome");
        }
    else{
        printf("Not");
       } 
        return 0;

}
**Armstrong Number**
#include<stdio.h>

int main() {
    int n, tem, r, sum = 0;
    printf("Enter any number: ");
    scanf("%d", &n);

    tem = n;
    while (tem != 0) {
        r = tem % 10;
        sum = sum + r * r * r;
        tem = tem / 10;
    }

    if (sum == n) {
        printf("Armstrong Number");
    } else {
        printf("Not Armstrong Number");
    }

    return 0;
}
//Counting number of a digit in an integer\\

#include<stdio.h>
int main()
{
    int n,count=0;

    printf("Enter Your digit : ");
    scanf("%d",&n);

    while(n!=0)
    {
        n=n/10;
        count++;
    }
    printf("Total number of digit:%d\n",count);
    return 0;
}

**Strong Number**
#include<stdio.h>
int main()
{
    int n,sum=0,r,tem,i,fact;

    printf("Enter a integer: ");
    scanf("%d",&n);

    tem=n;
    while(tem!=0)
    {
        r=tem%10;
        fact=1;
        for(i=1;i<=r;i++)
        {
            fact=fact*i;
        }

        sum=sum+fact;
        tem=tem/10;
    }
    if(sum==n){
        printf("%d is Strong number ",n);
    }else
    {
         printf("%d is not Strong number ",n);
    }
    return 0;
}

**  Series – 1**
#include<stdio.h>
int main()
{
    int n,i,sum=0;
    printf("Enter the last digit: ");
    scanf("%d",&n);
    printf("1+3+5+.....+%d",n);

    for(i=1;i<=n;i=i+2)
    {
        sum=sum+i;
    }
    printf("=%d\n",sum);
    return 0;
}
**  Series – 2**
#include<stdio.h>
int main()
{
    int n,a=1,sum=0;
    printf("Enter the last digit: ");
    scanf("%d",&n);
    printf("1+2+3+.....+%d",n);

   while(a<=n)
    {
        sum=sum+a;
        a=a+1;
    }
    printf("=%d\n",sum);
    return 0;
}
**SUM of Even Number**
#include<stdio.h>
int main()
{
    int i,n,sum=0;
    printf("Entre your Number: ");
    scanf("%d",&n);

    for(i=2;i<=n;i=i+2)
    {

       printf("%d ",i);
       sum=sum+i;
    }
    printf("\nSum = %d\n",sum);
    return 0;

}
**Maximum and Minimum of Array**
#include<stdio.h>

int main() {
    int num[1000], n, i;

    printf("How many Numbers: ");
    scanf("%d", &n);

    for(i = 0; i < n; i++) {
        scanf("%d", &num[i]);
    }

    int max = num[0];
    int maxIndex = 0;

    for(i = 1; i < n; i++) {
        if (max < num[i]) {
            max = num[i];
            maxIndex = i;
        }
    }

    printf("Maximum variable = %d\n", max);
    printf("Position (index) of maximum variable = %d\n", maxIndex+1);

    return 0;
}

Array | Searching a number (Linear search)
#include<stdio.h>
int main()
{
    int num[9]={10,5,17,18,90};
    int value,pos=-1,i;
    printf("Enter the value you want to search: ");
    scanf("%d",&value);

    for(i=0;i<9;i++)
        {
            if(value==num[i])
            {
                pos=i+1;
                break;
            }
        }

    if(pos==-1)
    {
        printf("Not Found");
    }
    else
    {
        printf("The poistion %d",pos);
    }
    return 0;
    }

    copy all elements of an array to another array

#include<stdio.h>

int main() {
    int array1[50], array2[50], i, n;

    printf("How many numbers: ");
    scanf("%d", &n);

    // Input elements for array1
    printf("Array1: ");
    for (i = 0; i < n; i++) {
        scanf("%d", &array1[i]);
    }

    // Display elements of array1
    printf("Array1: ");
    for (i = 0; i < n; i++) {
        printf("%d ", array1[i]);
    }

    // Copy elements from array1 to array2
    for (i = 0; i < n; i++) {
        array2[i] = array1[i];
    }

    // Display elements of array2
    printf("\nArray2: ");
    for (i = 0; i < n; i++) {
        printf("%d ", array2[i]);
    }

    return 0;
}

2D Array

#include<stdio.h>

int main() {
    int i, j;
    int A[3][4];

    // Input
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 4; j++) {
            scanf("%d", &A[i][j]); // Add & before A[i][j]
        }
    }

    // Output
    for(i = 0; i < 3; i++) {
        for(j = 0; j < 4; j++) {
            printf("%d ", A[i][j]); // Print a space after each element
        }
        printf("\n"); // Add a newline after each row
    }

    return 0;
}

Simple Matrix
#include<stdio.h>

int main() {
    int i, j;
    int A[3][4],B[3][4];

    // Input A
    printf("Enter elements For A Matrix. ");
    for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 4; j++)
        {
            printf("A[%d][%d]= ",i,j);
            scanf("%d", &A[i][j]); // Add & before A[i][j]
        }
        printf("\n");
    }

    printf("A= ");
    // Output for A matrix
    for(i = 0; i < 3; i++)
    {
        printf("\t");
        for(j = 0; j < 4; j++) {
            printf("%d ", A[i][j]); // Print a space after each element
        }
        printf("\n"); // Add a newline after each row
    }


    // Input B
    printf("Enter elements For b Matrix.");
    for(i = 0; i < 3; i++)
    {
        for(j = 0; j < 4; j++)
        {
            printf("B[%d][%d]= ",i,j);
            scanf("%d", &B[i][j]); // Add & before A[i][j]
        }
        printf("\n");
    }

    printf("B=");
    // Output for A matrix
    for(i = 0; i < 3; i++)
    {
        printf("\t");
        for(j = 0; j < 4; j++) {
            printf("%d ", B[i][j]); // Print a space after each element
        }
        printf("\n"); // Add a newline after each row
    }

    return 0;
}

# beeecrowed
1000
#include<stdio.h>
int main()
{  
    printf("Hello World!\n");
    return 0;
}
1001
#include <stdio.h>
 
int main() { 
    int A, B, X;

    scanf("%d", &A);
    scanf("%d", &B);

    X=A+B;

    printf("X = %d\n", X);

    return 0;
}
1002
#include <stdio.h>
int main()
{
    double A,R,n;
    n=3.14159;
    scanf("%lf",&R);
    A=n*R*R;
    printf("A=%.4lf\n",A);
    return 0;
}

1003
#include <stdio.h>
int main()
{
    int A,B,x;
    scanf("%d %d",&A,&B);
    x=A+B;
    printf("SOMA = %d\n",x);
    return 0;
}
1004
#include <stdio.h>
int main()
{
    int A,B,x;
    scanf("%d %d",&A,&B);
    x=A*B;
    printf("PROD = %d\n",x);
    return 0;
}
1005
#include <stdio.h>
int main()
{
    double A,B,x,y;
    scanf("%lf %lf",&A,&B);
    x=A*3.5+B*7.5;
    y=x/11;
    printf("MEDIA = %.5lf\n",y);
    return 0;
}

1006
#include <stdio.h>
int main()
{
    double A,B,C,x,y;
    scanf("%lf %lf %lf",&A,&B,&C);
    x=A*2+B*3+C*5;
    y=x/10;
    printf("MEDIA = %.1lf\n",y);
    return 0;
}
1007
#include <stdio.h>
int main()
{
    int A,B,C,D,x;
    scanf("%d %d %d %d",&A,&B,&C,&D);
    x=(A*B)-(C*D);
    printf("DIFERENCA = %d\n",x);
    return 0;
}
1008
#include <stdio.h>
int main()
{
    int number,wh;
    float pwh;
    double ts;
    scanf("%d %d %f",&number,&wh,&pwh);
    printf("NUMBER = %d\n",number);
    ts=wh*pwh;
    printf("SALARY = U$ %.2lf\n",ts);
    return 0;
}

1010
#include<stdio.h>
int main()
{
    int code1,unit1,code2,unit2;
    float p1,p2,tp;
    scanf("%d %d %f",&code1,&unit1,&p1);
    scanf("%d %d %f",&code2,&unit2,&p2);

    tp=(unit1*p1)+(unit2*p2);
    printf("VALOR A PAGAR: R$ %.2f\n",tp);
    return 0;
}
1016

#include<stdio.h>
int main()
{
    int km,dis;
    scanf("%d",&km);
    dis=km*2;
    printf("%d minutos\n",dis);
    return 0;
}

1043

#include<stdio.h>
int main()
{
   float a,b,c;
    scanf("%f%f%f",&a,&b,&c);
    if((a+b)>c&&(b+c)>a &&(c+a)>b)
    {
        printf("Perimetro = %.1f\n",(a+b+c));
    }
    else{
        printf("Area = %.1f\n",((a+b)*c/2));
    }
    return 0;

}


1052
#include <stdio.h>

int main()
{
    int x;
    scanf("%d",&x);
    if(x==1){printf("January\n");}
    else if(x==2){printf("February\n"); }
    else if(x==3){printf("March\n");}
    else if(x==4){printf("April\n");}
    else if(x==5){printf("May\n");}
    else if(x==6){printf("June\n");}
    else if(x==7){printf("July\n");}
    else if(x==8){printf("August\n");}
    else if(x==9){printf("September\n");}
    else if(x==10){printf("October\n");}
    else if(x==11){printf("November\n");}
    if (x==12){printf("December\n");}
    return 0;
}
1062
#include <stdio.h>

int main() {
    int num, even = 0, odd=0, positive= 0,negative=0;

    for (int i = 0; i < 5; i++) {
        scanf("%d", &num);

        if (num % 2 == 0) {
            even++;
        } else {
            odd++;
        }

        if (num > 0) {
            positive++;
        } else if (num < 0) {
            negative++;
        }
    }

    printf("%d valor(es) par(es)\n", even);
    printf("%d valor(es) impar(es)\n", odd);
    printf("%d valor(es) positivo(s)\n", positive);
    printf("%d valor(es) negativo(s)\n", negative);

    return 0;
}



codeforce  watermalon
#include<stdio.h>
int main()
{
    int w;
 
    scanf("%d",&w);
    if(w%2==0 && w>2)
        printf("Yes\n");
    else printf("No\n");
}
Fibonacci series 
#include<stdio.h>

int main() {
    int a[100], n, i;

    printf("How many Numbers: ");
    scanf("%d", &n);

    a[0]=0;
    a[1]=1;

    for(i = 2; i < n; i++)
    {
        a[i]=a[i-1]+a[i-2];
    }
    printf("\n");
      for(i = 0; i < n; i++)
      {
          printf("%d ",a[i]);
      }

      return 0;
}
