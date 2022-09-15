## 1026 : [기초-입출력] 시분초 입력받아 분만 출력하기(설명)


입력되는 시:분:초 에서 분만 출력해보자.

참고
int h, m, s;
scanf("%d:%d:%d", &h, &m, &s);
를 실행하면 콜론을 사이에 둔 형식으로 입력되어, h, m, s에 각각 정수값만 저장된다.


입력
시 분 초가
시:분:초 형식으로 입력된다.

출력
분만 출력한다.

입력예시
17:23:57


출력예시
23

```shell
import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		String cmd[] = sc.nextLine().split(":");
		
		System.out.println(Integer.valueOf(cmd[1]));
		
	}

}
```
.spilt를 이용해서 시 분 초 를 나눠주고 cmd에 저장을 하는데 cmd에 저장하는 시간은 문자이기 때문에 이걸 정수로 바꿔주기 위해 Integer.valueOf()를 사용한다. 
