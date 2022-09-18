### 1032 : [기초-출력변환] 10진 정수 입력받아 16진수로 출력하기1(설명)


10진수를 입력받아 16진수(hexadecimal)로 출력해보자.

참고
%d(10진수 형태)로 입력받고
%x로 출력하면 16진수(hexadecimal) 소문자로 출력된다.

10진법은 한 자리에 10개(0 1 2 3 4 5 6 7 8 9)의 문자를 사용하고,
16진법은 한 자리에 16개(0 1 2 3 4 5 6 7 8 9 a b c d e f)의 문자를 사용한다.
16진수의 a는 10진수의 10, b는 11, c는 12 ... 와 같다.

![pimg6148_1](https://user-images.githubusercontent.com/105026909/190911073-f64dfc8a-2ac6-4e9b-bb5c-a95f69e1d16f.png)


입력
10진수 1개가 입력된다.

출력
16진수(소문자)로 출력한다.

입력예시
255

출력예시
ff

```
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int a = sc.nextInt();

		System.out.println(Integer.toHexString(a));


	}

}
```

10진수에서 16진수로 바꿀때는 integer.toHexString();를 사용하고 반대로
16진수에서 10진수로 바꿀때는 Integer.parseint(String s , int radix); 사용하면 된다.

