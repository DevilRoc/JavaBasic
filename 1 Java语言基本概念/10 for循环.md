求最大公约数和最小公倍数
```java
import java.util.Scanner;
//求两个正整数的最大公约数和最小公倍数
public class ForTest {
    public static void main(String[] args) {
        System.out.println("请输入第一个整数:");
        int m = new Scanner(System.in).nextInt();
        System.out.println("请输入第二个整数:");
        int n = new Scanner(System.in).nextInt();
        int max = Math.max(m, n);
        int min = Math.min(m, n);
        //用最小的数去遍历取模求最大公约数
        for (int i = min; i >= 1; i--) {
            if (m % i == 0 && n % i == 0) {
                System.out.println("最大公约数是" + i);
                break;
            }
        }
        //用最大的数去遍历取模求最大公倍数
        for (int i = max; i <= m * n; i++) {
            if (i % m == 0 && i % n == 0) {
                System.out.println("最大公倍数为" + i);
                break;
            }
        }
    }
}

```