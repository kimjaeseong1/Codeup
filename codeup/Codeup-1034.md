## 1034 : [기초-출력변환] 8진 정수 1개 입력받아 10진수로 출력하기(설명)

﻿
8진수로 입력된 정수 1개를 10진수로 바꾸어 출력해보자.

참고

%o로 입력받으면 8진수로 인식시켜 저장시킬 수 있다.
%d로 출력하면 10진수로 출력된다.

예시

int n;
scanf("%o", &n);
printf("%d", n);
(C언어에서 소스 코드 작성 시 0으로 시작하는 수는 8진수로 인식된다. int a = 013; // 10진수 11과 같은 값)

![화면 캡처 2022-09-28 172409](https://user-images.githubusercontent.com/105026909/192728359-8fde369b-8db9-4375-a5f0-701810b944e0.png)


입력
8진 전수 1개가 입력된다.

출력
10진수로 바꾸어 출력한다.

입력예시
13

출력 예시
11

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		String a = sc.nextLine();


		System.out.println(Integer.valueOf(a, 8));


	}

}
```
2진수 -> 10진수 변환 : Integer.valueOf(String,2);
8진수 -> 10진수 변환 : Integer.valueOf(String,8);
16진수 -> 10진수 변환 : Integer.valueOf(String,10);

10진수를 2진수 ,8진수,16진수로 변환
10진수 -> 2진수 변환 : Integer.toBinaryString(int)
10진수 -> 8진수 변환 : Integer.toOctalString(int)
10진수 -> 16진수 변환 : Integer.toHexString(int)

