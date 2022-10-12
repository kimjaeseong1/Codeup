## 1037 : [기초-출력변환] 정수 입력받아 아스키 문자로 출력하기


10진 정수 1개를 입력받아 아스키 문자로 출력해보자.

단, 0 ~ 255 범위의 정수만 입력된다.

![화면 캡처 2022-10-12 213150](https://user-images.githubusercontent.com/105026909/195343536-339b86b5-f482-42db-9b15-1d5dbae5b37e.png)


입력

10진 정수 1개(0 ~ 255 범위)가 입력된다.


출력

아스키코드 값을 문자로 출력한다.


입력예시

65


출력예시

A

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int a = sc.nextInt();
		char b = (char)a;
		
		System.out.println(b);
		
		
	}

}

```
10진수 정수를 받은다음 문자 하나니까 char자료형으로 캐스팅을 해서 b에 저장을 한다.