# no.-of-pattern-using-recursion.c
important for clear understanding.// C program to print pattern using recursion in functions with numbers      1    121   12312  1234123 123451234 
// C program to print pattern using recursion in functions with numbers

    1
   121
  12312
 1234123
123451234


#include <stdio.h>
void fun(int);
void funs(int);
void funj(int);
void funj1(int);

int main() {
    int i,j,s;
    fun(4);
    return 0;
}
    void fun(int i)
    {
    if (i==-1)
    return;
    fun(i-1);
    funs(3-i);
    funj(i);
    funj1(i-1);
    printf("\n");
}
    void funs(int s)
    {
        if(s==-1)
        return;
        funs(s-1);
        printf(" ");
    }
    void funj(int j)
    {
        if(j==-1)
        return;
        funj(j-1);
        printf("%d",1+j);
    }
    void funj1(int j)
    {
        if(j==-1)
        return;
        funj1(j-1);
        printf("%d",1+j);
    }
