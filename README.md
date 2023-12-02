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
