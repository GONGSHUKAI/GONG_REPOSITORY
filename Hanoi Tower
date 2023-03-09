#include <stdio.h>
static int count=0;
void step_print(int m,char place1,char place2)
{
    count++;
    printf("[step %d] move plate %d# from %c to %c\n",count,m,place1,place2);
}

void hannoi(int n,char start,char middle,char end)
{
    if (n==1)
    {
        step_print(n,start,end);
    }
    else
    {
        hannoi(n-1,start,end,middle);
        step_print(n,start,end);
        hannoi(n-1,middle,start,end);
    }
}

int main()
{
    int number;
    scanf("%d",&number);
    hannoi(number,'a','b','c');
    printf("%d\n",count);
    return 0;
}
