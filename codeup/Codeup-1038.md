## 1038 : [기초-산술연산] 정수 2개 입력받아 합 출력하기1(설명)

정수 2개를 입력받아 합을 출력하는 프로그램을 작성해보자.

(단, 입력되는 정수는 -1073741824 ~ 1073741824 이다.)

![화면 캡처 2022-10-12 213459](https://user-images.githubusercontent.com/105026909/195343959-09bcbd8e-88a5-4f71-96d6-ab6b9f419215.png)


입력

2개의 정수가 공백으로 구분되어 입력된다.

`**주의 : 계산의 결과가 int 범위를 넘어가는지를 잘 생각해 보아야 한다.
`


출력

`두 정수의 합을 출력한다.`


입력예시

`123 -123`


출력예시

`0`

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		long a = sc.nextLong();
		
		long b = sc.nextLong();
		long c = a+b;
		
		System.out.println(c);
		
		
	}

}
```
