## 1095 : [기초-1차원배열] 이상한 출석 번호 부르기3(설명)

정보 선생님은 오늘도 이상한 출석을 부른다.

​

영일이는 오늘도 다른 생각을 해보았다.

출석 번호를 다 부르지는 않은 것 같은데... 가장 빠른 번호가 뭐였지?

​

출석 번호를 n번 무작위로 불렀을 때, 가장 빠른 번호를 출력해 보자.

​

​

참고

배열에 순서대로 기록해 두면, 기록된 내용을 모두 검사해 가장 작은 값을 찾아내면 된다.

​

그런데, 가장 작은 값은 어떻게 어떤 것과 비교하고 찾아야 할까?

​
<img src="https://codeup.kr/upload/pimg6211_1.png">








입력

>번호를 부른 횟수(n, 1 ~ 10000)가 첫 줄에 입력된다.
> 
> n개의 랜덤 번호(k, 1 ~ 23)가 두 번째 줄에 공백을 사이에 두고 순서대로 입력된다.





출력

>출석을 부른 번호 중에 가장 빠른 번호를 1개만 출력한다.

입력 예시

>10
>
>10 4 2 3 6 6 7 9 8 5

​


출력예시
2


```shell
import java.util.Scanner;


public class pra0921 {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        int a = sc.nextInt();
        int min = 24;
        int[] num = new int[a];

        for(int i=0; i<a; i++){
             num[i] =  sc.nextInt();
        }

        for(int i=0; i<num.length; i++){
            if(min>num[i]){
                min=num[i];
            }
        }
        System.out.println(min);
    }
}
```
