## 1063 : [기초-삼항연산] 두 정수 입력받아 큰 수 출력하기(설명)

입력된 두 정수 a, b 중 큰 값을 출력하는 프로그램을 작성해보자.

단, 조건문을 사용하지 않고 3항 연산자 ? 를 사용한다.


참고

3개의 요소로 이루어지는 3항(ternary) 연산자는

"조건식 ? (참일 때의 값) : (거짓일 때의 값)” 의 형태로 사용하는 연산자이다.

- 조건식의 계산 결과가 참인 경우에는 ':' 왼쪽의 값 또는 식으로 바뀌고,

- 거짓인 경우에는 ':' 오른쪽의 값 또는 식으로 바뀐다.


예를 들어

123 > 456 ? 0 : 1

과 같은 표현식은 123 > 456 의 비교연산 결과가 거짓이므로 1이 된다.


예시

printf("%d", a>b ? a:b); //두 값 중 큰 값이 출력된다.


예시 코드는 a>b 의 결과가 참(1)이면 (a>b ? a:b)의 결과는 a가 되고,

거짓(0)이면 (a>b ? a:b)의 결과는 b가 된다.


<img src="https://codeup.kr/upload/pimg6179_1.png">





입력

>2개의 정수가 공백을 두고 입력된다. 
> 
> -2147483648 ~ +2147483647


출력

>두 정수 중 큰 값을 10진수로 출력한다.

입력 예시

>123 456

출력예시

>456

```shell
import java.util.Scanner;

public class test {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int b = sc.nextInt();
        System.out.println(a>b? a:b);

    }
}


```