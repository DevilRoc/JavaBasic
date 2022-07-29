```java
import java.util.Scanner;
public class switchCaseTest {
    public static void main(String[] args) {
        System.out.println("请输入成绩:");
        int score = new Scanner(System.in).nextInt();
        switch (score / 10) {
            case 0, 1, 2, 3, 4, 5 -> System.out.println("不及格");//增强型case自带break
            case 6, 7, 8, 9, 10 -> System.out.println("及格");
            default -> throw new RunTimeException("输入非法");
        }
    }
}
```
### 计算一年当中的第几天
```java
import java.util.Scanner;
public class SwitchCaseTest {
    public static void main(String[] args) {
        System.out.println("请输入年份:");
        int year = new Scanner(System.in).nextInt();
        System.out.println("请输入月份:");
        int month = new Scanner(System.in).nextInt();
        System.out.println("请输入日期:");
        int date = new Scanner(System.in).nextInt();
        int sumDays = 0;

        switch (month) {//switch case可以解决冗余问题
            case 12:
                sumDays += 30;
            case 11:
                sumDays += 31;
            case 10:
                sumDays += 30;
            case 9:
                sumDays += 31;
            case 8:
                sumDays += 30;
            case 7:
                sumDays += 30;
            case 6:
                sumDays += 31;
            case 5:
                sumDays += 30;
            case 4:
                sumDays += 31;
            case 3:
                if ((year % 4 == 0 && year % 100 != 0) || (year % 400 == 0)) {//判断是否是闰年
                    sumDays += 29;
                }else {
                    sumDays += 28;
                }
            case 2:
                sumDays += 31;
            case 1 :
                sumDays += date;
                break;
            default:
                throw new RuntimeException("输入非法");
        }
        System.out.println(year + "年" + month + "月" + date + "日" + "是一年当中的第" + sumDays + "天");
    }
}

```
