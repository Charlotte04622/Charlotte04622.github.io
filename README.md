# Charlotte04622.github.io
hello! welcome!

# 整數的差別
```cpp
#include<stdio.h>
int main()
{
    int n=9876543210;
    printf("int 印出來 %d\n", n);

    long long int a=9876543210;
    printf("long long int 印出來 %lld\n", a);
}
```
# long long int 很長很長的整數計算
```cpp
#include<stdio.h>
 int main()
 {

     long long int a, b;
     scanf("%lld %lld", &a, &b);

     long long int ans;
     for(long long int i = 1; i<=a; i++){
        if( a%i==0 && b%i==0 ) ans = i;


     }
     printf("最大公因數是:%lld\n", ans);
 }
```
# 輾轉相除法
```cpp
#include<stdio.h>
 int main()
 {

     long long int a, b, c;
     scanf("%lld %lld", &a, &b);
     while(1){
        c = a % b;
        printf("a:%lld b:%lld c:%lld\n", a, b, c);
        if(c==0)break;
        a=b;
        b=c;
     }
    printf("答案是: %lld\n",b);
 }
```
# 剝皮
```cpp
#include<stdio.h>
 int main()
{
    int n;
    scanf("%d", &n);

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;\

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

    printf("現在個位數:%d\n",n%10);
    n = n / 10;

}

# week08
```
#判斷1個質數
```cpp
#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);
    int bad=0;
    for(int i=2; i<n; i++){
        if( n%i==0 ) bad=1;
    }
    if(bad==0)printf("%d 是質數",n );
    else printf("%d不好, 不是質數", n);
}

```
#列出質數
```cpp
#include <stdio.h>
int main()
{
    printf("請輸入五個數字(要加起來):");

    int n;
    int sum=0;
    for(int i=0; i<5; i++){
        scanf("%d",&n);
        sum+= n;
    }
    printf("總呵是:%d",sum);
}

```
#直角三角形
```cpp
#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);

    for(int i=1;i<=n;i++){

        for(int k=1; k<=n-i;k++)printf(" ");

        for(int k=1; k<=i;k++)printf("*");

        printf("\n");
    }
}
```
#while迴圈
```cpp
#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);

    for(int i=1;i<=n;i++){

        for(int k=1; k<=n ;k++){

            if(k<=n-i)printf(" ");
            else      printf("*");
        }
        printf("\n");
    }
}

```
#有星星的右方直角三角形
```cpp
#include <stdio.h>
int main()
{
    int n;
    scanf("%d", &n);

    int i=1;
    while(i<=n){

            int k=1;
            while(k<=n){

                if(k<=n-i)printf(" ");
                else printf("*");

                k++;
    }
    printf("\n");
    i++;
    }

}



 

