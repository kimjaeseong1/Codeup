## 1058 : [기초-논리연산] 둘 다 거짓일 경우만 참 출력하기
두 개의 참(1) 또는 거짓(0)이 입력될 때,

모두 거짓일 때에만 참이 계산되는 프로그램을 작성해보자.

<img src="https://codeup.kr/upload/pimg6174_1.png">





입력

>1또는 0의 값만 가지는 2개의 정수가 공백을 두고 입력된다.


출력

>둘 다 거짓일 경우에만 1을 출력하고, 그 외의 경우에는 0을 출력한다.

입력 예시

>0  1

출력예시

>0


```shell
import java.util.Scanner;

public class test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();

        if(a==0 && b==0){
            System.out.println(1);
        }else{
            System.out.println(0);
        }
    }
}

```
