```java
public class VariableTest {
    public static void main(String[] args) {
        byte b1 = 127;
        short s1 = 32767;
        char c1 = 97;
        int i1 = b1 + s1 + c1;//byte,short,char会自动转换成int来进行计算
        float f1 = i1;//整型转浮点,可能会精度损失
        float f2 = f1 + f1;//float + float还是float
        double d1 = f1 + 12.3;//float + double 是double

        int i2 =(int)f1; //浮点转整型会截断

        int i3 = 128;
        byte b2 = (byte)i3; //大的整型通过强制类型转换放入小的整型,可能会发生循环

        String string1 = "7231";
        int i4 = Integer.parseInt(string1);//Integer工具类使用parseInt强转字符串
        double d2 = Double.parseDouble(string1);//Double工具类使用parseDouble()强制转换字符串
    }
}
```
