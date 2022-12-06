## 1075 : [기초-반복실행구조] 정수 1개 입력받아 카운트다운 출력하기2(설명)
정수(1 ~ 100) 1개가 입력되었을 때 카운트다운을 출력해보자.

​

​

예시

int n;

scanf("%d", &n);

while(n!=0)

{

n=n-1; //n--; 와 같다.

printf("%d", n);

}

<img src="https://codeup.kr/upload/pimg6191_1.png">








입력

>정수 1개가 입력된다.
>
> (1 ~ 100)




출력

>1씩 줄이면서 한 줄에 하나씩 0이 될 때 까지 출력한다.


입력 예시

>5



출력예시

4

3

2

1

0


```shell

import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int a = sc.nextInt();

        while(a!=0){
            System.out.println(a-1);
            a--;
        }

    }
}
```
