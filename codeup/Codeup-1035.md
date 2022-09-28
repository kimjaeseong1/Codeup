## 1035 : [기초-출력변환] 16진 정수 1개 입력받아 8진수로 출력하기(설명)

16진수로 입력된 정수 1개를 8진수로 바꾸어 출력해보자.

참고

%x(영문자 소문자) 나 %X(영문자 대문자)로 입력 받으면
16진수로 인식시켜 저장시킬 수 있다. %o로 출력하면 8진수로 출력된다.
C언어에서 소스 코드 작성시 0으로 시작하는 수는 8진수로 인식된다.
또한 소스코드 내에서 //로 시작하면 1줄 설명을 넣을 수 있다.
여러 줄을 설명(주석) 을 넣을 경우 /* 와 */ 사이에 작성하면 된다.

예시

int n;
scanf("%x", &n); //소문자로 16진수 입력
printf("%o", n);

![화면 캡처 2022-09-28 172735](https://user-images.githubusercontent.com/105026909/192729164-dc46598d-47f2-4bb0-8a20-6f7b82e31ade.png)


입력
16진수 전수 1개가 입력된다.
(단, 16진수는 영문 소문자로 입려된다.)

출력
8진수로 바꾸어 출력한다.

입력예시
f

출력예시
17

```shell
package Text;

import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		String a = sc.nextLine();
		int b = Integer.parseInt(a, 16); //10진수 변환

		System.out.println(Integer.toOctalString(b)); // 8진수로 변환해서 출력

	}

}
```
16진수를 입력을 받고 10진수로 변환 후 8진수로 변화하는 과저으로 해결
