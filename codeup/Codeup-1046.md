##  1046 : [기초-산술연산] 정수 3개 입력받아 합과 평균 출력하기

정수 3개를 입력받아 합과 평균을 출력해보자.

단, -2147483648 ~ +2147483647

![pimg6162_1](https://user-images.githubusercontent.com/105026909/198195298-a06c3c6a-30b4-467c-95de-edca0e4c85e5.png)



입력


정수 3개가 공백을 두고 입력된다.

단, -2147483648 ~ +2147483647


출력

합과 평균을 줄을 바꿔 출력한다.

평균은 소수점 이하 둘째 자리에서 반올림해서 소수점 이하 첫째 자리까지 출력한다.

입력예시

1 2 3

출력예시

6

2.0

```shell
import java.util.Scanner;

public class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        long sum =0;
        double avg = 0.0;

        long a = sc.nextLong();
        long b = sc.nextLong();
        long c= sc.nextLong();

        sum = a+b+c;
        avg =sum/3.0;

        System.out.println(sum);
        System.out.printf("%.1f" ,avg);
    }   
} 

```
소수점 이하 둘째 자리에서 반올림해서 소수점 이하 첫째 자리까지 출력해야 하니까 printf를 사용해서 .1f를 하면 소수점 이하 첫째자리까지 출력 됨