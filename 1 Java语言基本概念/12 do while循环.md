```java
//遍历并输出100以内的偶数
public class DoWhileTest {
    public static void main(String[] args) {
        int i = 1;
        do {
            if (i++ % 2 == 0) {
                System.out.println(i);
            }
        } while (i <= 100);
    }
}

```