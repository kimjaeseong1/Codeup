## 1033 : [기초-출력 변환] 10진 정수 입력받아 16진수로 출력하기 2(설명)

10진수를 입력받아 16진수(hexadecimal)로 출력해 보자.

참고

%d(10진수 형태)로 입력받고
%X로 출력하면 16진수(hexadecimal) 대문자로 출력된다.
10진법은 한자리에 10개(0 1 2 3 4 5 6 7 8 9)의 문자를 사용하고,
16진법은 한자리에 16개(0 1 2 3 4 5 6 7 8 9 A B C D E F)의 문자를 사용한다.
(알파벳 대소문자는 표현만 다르고 같은 값을 의미한다.)
16진 법의 A는 10진 법의 10, B는 11, C는 12 ... 와 같다.

![화면 캡처 2022-09-28 171926](https://user-images.githubusercontent.com/105026909/192727299-2caea1b2-93f3-469b-bdce-23f8fabfeb26.png)

입력
10진수 1개가 입력된다.

출력
16진수(대문자)로 출력한다.

입력 예시
255

출력 예시
FF

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int a = sc.nextInt();
		String b = Integer.toHexString(a);

		System.out.println(b.toUpperCase());


	}

}
```
소문자를 대문자로 바꿀 때는 to.UpperCase();를 사용을 하고
대문자를 소문자를 바꿀 때는 to.lowerCase();를 사용을 한다.


