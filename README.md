#include<stdio.h>
int main(){
    float num1,num2,result;
    char op;

    printf("enter first number:");
    scanf("%f" , &num1);

    printf("enter operator(+,-,*,/):");
    scanf(" %c" , &op);

    printf("enter second number:");
    scanf("%f" , &num2);

    switch(op)
    {
        case'+':
        result=num1+num2;
        printf("result=%2f",result);
        break;

        case'-':
        result=num1-num2;
        printf("result=%2f",result);
        break;

        case'*':
        result=num1*num2;
        printf("result=%2f",result);
        break;

        case'/':
        if(num2!=0)
        {
             result=num1/num2;
        printf("result=%2f",result);
        }
       else{
        printf("cannont divide by zero.");
       }
       break;

       default:
       printf("invalid operator!");
    }
    return 0;
}
