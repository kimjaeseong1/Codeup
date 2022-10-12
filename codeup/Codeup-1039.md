## 1039 : [기초-산술연산] 정수 2개 입력받아 합 출력하기2(설명)

정수 2개를 입력받아 합을 출력해보자.

단, 입력되는 정수는 -2147483648 ~ +2147483648 이다.


참고

- `+ 연산자`를 사용하면 된다.

단, 계산된 결과가 int 형으로 저장할 수 있는 범위를 넘어갈 수 있기 때문에 다른 데이터형을 사용해야 한다.


주의

int 데이터형은 %d로 입출력하고,

long long int 데이터형은 %lld로 입출력한다.

![화면 캡처 2022-10-12 213737](https://user-images.githubusercontent.com/105026909/195344389-b10a40a5-bccd-4056-9b9f-2f2eb3bfa183.png)


입력

`2개의 정수가 공백으로 구분되어 입력된다.`


출력

`두 정수의 합을 출력한다.`


입력예시

`2147483648 2147483648`


출력예시

`4294967296`

```shell
import java.util.Scanner;

public class Example {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		long a = sc.nextLong();
		
		long b = sc.nextLong();
	
		
		System.out.println(a+b);
		
		
		
	}

}
```