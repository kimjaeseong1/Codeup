## 1036 : [기초-출력변환] 영문자 1개 입력받아 10진수로 출력하기(설명)

영문자 1개를 입력받아 아스키 코드표의 10진수 값으로 출력해보자.


참고
아스키 코드는
(ASCII, 미국표준코드, American Standard Code for Information Interchange)
영문자, 특수문자 등을 저장할 때 사용하는 표준 코드이다.
컴퓨터로 저장되는 모든 데이터는 2진 정수화되어 저장되는데,
영문자와 특수기호 등을 저장하는 방법으로 아스키코드가 기본적으로 사용된다.

예를 들어 영문 대문자 "A"는 10진수 65를 의미하는 2진수 값으로 저장된다.


![화면 캡처 2022-09-28 173132](https://user-images.githubusercontent.com/105026909/192730078-70df55fd-edfd-46d6-a59a-c59913ca7a58.png)

입력
영문자 1개가 입력된다.

출력
아스키코드 값을 10진수로 출력한다.

입력예시
A

출력예시
65

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		char a = sc.next().charAt(0);

		System.out.println((int)a);


	}

}
```

Scanner는 String으로만 문자를 받을 수 있어서 .charAt(원하는 인덱스) a 하나밖에 없으니 0으로 해준다 . 만약 배열로 저장을 한다면 바꾸고 싶은 인덱스 번호를 입력을 해준다 .
그리고 int로 캐스팅해서 출력을 하면 해결!


