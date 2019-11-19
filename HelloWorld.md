# 查找指定字符

``` C
#include<stdio.h>
int main()
{
    char ls[100];
    char ch;
    int cnt = 0 , flag = 0 , count = 0;
    ch = getchar();
    getchar();
    scanf("%[^\n]",ls);
    while(ls[cnt]){
        if (ls[cnt] == ch){
            count = cnt;
            flag = 1;
        }
        cnt ++;
    }
    if (flag){
        printf("index = %d",count);
    }else{
        printf("Not Found");
    }
}
```
