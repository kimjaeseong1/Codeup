## 1027 : [기초-입출력] 년월일 입력 받아 형식 바꿔 출력하기(설명)

년월일을 출력하는 방법은 나라마다, 형식마다 조금씩 다르다.
년월일(yyyy.mm.dd)를 입력받아,
일월년(dd-mm-yyyy)로 출력해보자.
(단, 한 자리 일/월은 0을 붙여 두자리로, 년도도 0을 붙여 네자리로 출력한다.)

참고
출력하는 자리수를 지정하기 위해 %4d와 같은 형식을 사용할 수 있는데,
빈칸을 0으로 출력하기 위해서는 %04d와 같은 형식을 사용하면 된다.

예시
printf("%02d-%02d-%04d", d, m, y);

입력
년월일이 '.'(닷)으로 구분되어 입력된다.

출력
년월일을
일월년으로 바꾸어 '-'(대쉬, 마이너스)로 구분해 출력한다.

입력예시
2014.07.15

출력예시
15-07-2014

```shell
import java.util.Scanner;

public class Main {

	public static void main(String[] args) {
		Scanner sc = new Scanner(System.in);
		String cmd[] = sc.nextLine().split("\\.");

		System.out.printf("%02d-%02d-%04d",Integer.valueOf(cmd[2]),Integer.valueOf(cmd[1]),Integer.valueOf(cmd[0]));


	}

}
```
.spilt으로 나눠주고 printf를 이용해서 숫자가 한자리가 나와도 07이렇게 두자리로 나와야 하기 때문에 02%d사용하고 년도는 %04d를 사용! 그리고 문자열로 저장을해서 Integer.valueOf를 이용해서 정수로 변환 하고 인덱스에 위치를 바꿔서 출력을 해준다 .
