```java
public class ifElse {
    public static void main(String[] args) {
        int x = 4;
        int y = 1;
        if (x > 2)
            if (y > 2)//不带花括号就输出一行语句
                System.out.println(x + y);
            else
                System.out.println("x的值为" + x);// x = 4
    }
}
```