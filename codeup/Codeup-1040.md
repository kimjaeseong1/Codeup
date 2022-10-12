## 1040 : [기초-산술연산] 정수 1개 입력받아 부호 바꿔 출력하기(설명)

입력된 정수의 부호를 바꿔 출력해보자.

단, -2147483647 ~ +2147483647 범위의 정수가 입력된다.



참고

단항 연산자인 -(negative)를 변수 앞에 붙이면 부호가 반대로 바뀌어 계산된다.



예시
```
int a;

scanf("%d", &a);

printf("%d", -a);

```

![pimg6156_1](https://user-images.githubusercontent.com/105026909/195344810-0135fd74-2516-459e-96d6-15ac8904a476.png)

입력

`정수 1개가 입력된다.`

출력

`부호를 바꿔 출력한다.`

입력예시

`-1`

출력예시

`1`

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		long a = sc.nextLong();
		
	
		
		System.out.println(-a);
		
		
		
	}

}
```
