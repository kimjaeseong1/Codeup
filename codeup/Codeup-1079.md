## 1079 : [기초-종합] 원하는 문자가 입력될 때까지 반복 출력하기
'q'가 입력될 때까지 입력한 문자를 계속 출력하는 프로그램을 작성해보자.


<img src="https://codeup.kr/upload/pimg6195_1.png">








입력

>문자들이 1개씩 계속해서 입력된다.




출력

>'q'가 입력될 때 까지 입력된 문자를 줄을 바꿔 한 줄씩 출력한다.


입력 예시

>X b k d i q g a c



출력예시

x

b

k

d

i

q

```shell

import java.util.Scanner;

public class pra0921 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        for(;;){
            char a = sc.next().charAt(0);
            System.out.println(a);
            if(a=='q'){

                return;
            }
        }
    }
}
```
