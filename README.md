#include <stdio.h>
long long  factor( long long x){
long long m=1;
int i;
for( i=1;i<=x;i++)
    m*=i;
return m;
}
int main ()
{
    long long  r,n;
    while(~scanf("%lld%lld",&r,&n)){
        printf("%lld\n",factor(r)/(factor(n)*factor(r-n)));
    }
    return 0;
}
