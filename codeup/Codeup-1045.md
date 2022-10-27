##  1045 : [기초-산술연산] 정수 2개 입력받아 자동 계산하기

정수 2개(a, b)를 입력받아 합, 차, 곱, 몫, 나머지, 나눈 값을 자동으로 계산해보자.

단 0 <= a, b <= 2147483647, b는 0이 아니다.

![pimg6161_1](https://user-images.githubusercontent.com/105026909/198195047-fadec202-6314-49b0-b5c9-65c0609b591a.png)


입력

정수 2개가 공백을 두고 입력된다.



출력

첫 줄에 합

둘째 줄에 차,

셋째 줄에 곱,

넷째 줄에 몫,

다섯째 줄에 나머지,

여섯째 줄에 나눈 값을 순서대로 출력한다.

(실수, 소수점 이하 셋째 자리에서 반올림해 둘째 자리까지 출력)



입력예시

10 3



출력예시

13

7

30

3

1

33.3

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int a = sc.nextInt();
		
		int b = sc.nextInt();
		
		

	      System.out.println(a+b);
	      System.out.println(a-b);
	      System.out.println(a*b);
	      System.out.println(a/b);
	      System.out.println(a%b);
	      System.out.printf("%.2f",Math.round((a/(double)b)*100)/100.00);
		}

}
```