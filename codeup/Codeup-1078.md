## 1078 : [기초-종합] 짝수 합 구하기(설명)
정수(1 ~ 100) 1개를 입력받아 1부터 그 수까지 짝수의 합을 구해보자.

​

​

참고

while( ) {...}, do {...} while( );, for(...; ...; ...) {...} 등의 반복문은 형태만 다르

고, 똑같은 성능을 발휘한다. 필요에 따라 편리한 것으로 골라 사용하면 된다.

​

예시

//아래의 예는 홀수일 경우만 더해 그 결과를 출력한다.

int sum=0;

int i, n;

scanf("%d", &n);

for(i=1; i<=n; i++)

{

if(i%2==1) sum=sum+i;

<img src="https://codeup.kr/upload/pimg6194_1.png">








입력

>정수 1개가 입력된다.
>
> ( 0 ~100)




출력

>1부터 입력된 수까지 짝수의 합을 출력한다.


입력 예시

>5



출력예시

6

```shell

import java.util.Scanner;

public class pra0921 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
       int a = sc.nextInt();
        int sum =0;
       for(int i =0; i<=a; i++){
          if(i%2==0){

              sum +=i;
          }
       }
        System.out.println(sum);
    }
}

```
