#include <stdio.h>
#include <math.h>

int main()
{
    float x;
    printf("\nInput x: ");
    scanf("%f", &x);
    if (x>5)
    {
        if (fabs(cos(fabs(x)))<1e-2)
        {
            printf("error. tg = infinity");
            return 1;
        }
    }

    else
    {
        if (sqrt(x)<0)
        {
            printf( " sqrt from <0 ");

        }

        if (-7*sqrt(x)+3==0)
        {
            printf(" div by 0 ");

        }

        if (sin(x)<1e-9)
        {
            printf(" Del 0 ");
            return 2;
        }



    }

    printf ("No errors.");
    return 0;
}
