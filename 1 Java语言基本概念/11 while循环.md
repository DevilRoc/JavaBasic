## 二分法搜索
```java

public class DichotomyTest {
    public static void main(String[] args) {
        int[] arr = new int[]{11, 22, 33, 44, 55, 66, 77, 88, 99};
        int dest = 22;
        //设置首末索引为指针, 求中间指针
        int head = 0;
        int end = arr.length - 1;
        boolean isFlag = true;
        //循环比较中间指针, 同时首末指针不能颠倒
        while (head <= end) {
            int middle = (head + end) / 2;
            if (dest == arr[middle]) {
                System.out.println("找到了指定元素, 索引为:" + middle);
                isFlag = false;
                break;
            } else if (dest < arr[middle]) {
                end = middle - 1;
            } else {
                head = middle + 1;
            }
        }
        if (isFlag) {
            System.out.println("没有找到指定元素");
        }
    }
}

```