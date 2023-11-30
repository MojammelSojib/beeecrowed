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
