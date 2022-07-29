```java
import java.util.Scanner;
public class ScannerTest {
    public static void main(String[] args){
        System.out.println("请输入您的性别(男/女):" );
        String gender = new Scanner(System.in).next();//匿名类
        char genderChar = gender.charAt(0);//字符串里的第一个字符
        System.out.println(genderChar);
    }
}
```