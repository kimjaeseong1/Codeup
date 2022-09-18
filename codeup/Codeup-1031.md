### 1031 : [기초-출력변환] 10진 정수 1개 입력받아 8진수로 출력하기(설명)


10진수를 입력받아 8진수(octal)로 출력해보자.

참고
%d(10진수 형태)로 입력받고,
%o를 사용해 출력하면 8진수(octal)로 출력된다.

![pimg6147_1](https://user-images.githubusercontent.com/105026909/190904384-6b58e0c5-4e12-4c10-925f-4117d42425d0.png)


입력
10진수 1개가 입력된다.
단, 입력되는 정수는 int 범위이다.

출력
8진수로 출력한다.


입력예시
10

출력예시
12

```
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		int a = sc.nextInt();

		System.out.printf("%o",a);


	}

}
```
