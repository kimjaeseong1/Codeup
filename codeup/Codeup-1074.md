## 1074 : [기초-반복실행구조] 정수 1개 입력받아 카운트다운 출력하기1(설명)
정수(1 ~ 100) 1개가 입력되었을 때 카운트다운을 출력해보자.


while(조건)

{

...

}

구조를 사용하자.


예시

int n;

scanf("%d", &n);

while(n!=0)

{

printf("%d", n);

n=n-1; //n--;와 같다.

}








입력

>정수 1개가 입력된다.
>
> (1 ~ 100)




출력

>1씩 줄이면서 한 줄에 하나씩 1이 될 때 까지 출력한다.


입력 예시

>5



출력예시

5

4

3

2

1



```shell

import java.util.Scanner;

public class pra0921 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();

        while(a>0){
            System.out.println(a);
            a--;
        }
    }
}
```
