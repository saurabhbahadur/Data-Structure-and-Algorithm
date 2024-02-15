<h1 align="center"> Introduction to 1D Array   </h1>
<p align="center" > () </p>

### Introduction of 1D Array
+ Linear Data Structure
+ Start index = 0
+ Last index = (n-1)
+ Total length = arr.length

### Palindrone
+ Palindrome comes from Greek palindromos, meaning `running back again` which itself is from palin ("back," "again") and dramein ("to run").

```java

public class demo {
    public static void main(String[] args) {
        int arr[] = { 4, 5, 4 };
        int n = arr.length;
        int flag = 0;
        for (int i = 0; i < n / 2; i++) {
            if (arr[i] != arr[n - i - 1]) {
                flag = 1;
                System.out.println("Number is not Palindrome");
                break;
            }
        }
        if (flag == 0) {
            System.out.println("Number is Palindrone");
        }

    }
}

```
```java

public class demo {
    public static void main(String[] args) {
        int r, sum = 0;
        int temp;
        int n = 12321;

        temp = n;
        while (n > 0) {
            r = n % 10;
            sum = (sum * 10) + r;
            n = n / 10;
        }
        if (temp == sum) {
            System.out.println("Number is Palindrome");
        } else {
            System.out.println("Number is not Palindrome");
        }

    }
}


```

### Pair
```java
public class demo {
    public static void pair(int num[]) {
        for (int i = 0; i < num.length; i++) {
            for (int j = i + 1; j < num.length; j++) {
                System.out.print("(" + num[i] + "," + num[j] + ")");
            }
            System.out.println("");
        }
    }

    public static void main(String[] args) {
        int num[] = { 1, 3, 5, 6, 8 };
        pair(num);
    }
}


```
```
// output
(1,3)(1,5)(1,6)(1,8)
(3,5)(3,6)(3,8)
(5,6)(5,8)
(6,8)

```

### Reversal in An Array

```java
public class demo {

    public static void reverse(int arr[]) {
        int n = arr.length;
        for (int i = 0; i < n / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[n - i - 1];
            arr[n - i - 1] = temp;
        }
    }

    public static void main(String[] args) {
        int arr[] = { 1, 2, 3, 4, 5 };
        reverse(arr);
        for (int i = 0; i < arr.length; i++) {
            System.out.println(arr[i]);
        }
    }
}
```

```java
public class demo {
    public static void reverse(int num[]) {
        int start = 0;
        int end = num.length - 1;
        while (start < end) {
            int temp = num[end];
            num[end] = num[start];
            num[start] = temp;

            start++;
            end--;
        }

    }

    public static void main(String[] args) {
        int num[] = { 1, 3, 5, 6, 8 };

        reverse(num);
        for (int i = 0; i < num.length; i++) {
            System.out.println(num[i]);
        }
    }
}


```

### Missing Numbers in an Array

```java
public class demo {
    public static void main(String[] args) {
        int arr[] = { 1, 2, 3, 5 };
        int n = arr.length;

        int sum_natural_num = ((n + 1) * (n + 2)) / 2;
        int sum = 0;

        for (int i = 0; i < n; i++) {
            sum = sum + arr[i];
        }
        int missing_ele = 0;
        missing_ele = sum_natural_num - sum;
        System.out.println(missing_ele);

    }
}

```

### Duplicate Elements Finding
```java
public class demo {
    public static void main(String[] args) {
        int arr[] = { 8, 1, 2, 3, 3, 5, 6, 7, 8 };
        int n = arr.length;
        for (int i = 0; i < n; i++) {
            for (int j = i + 1; j < n; j++) {
                if (arr[i] == arr[j]) {
                    System.out.println(arr[i]);
                }
            }
        }
    }
}

```



***

# Feel Free to connect
+ ### [LinkedIn](https://www.linkedin.com/in/saurabhbahadur)
+ ### [Mail](mailto:singhsaurabhbahadur@gmail.com)
+ ### [Instagram](https://www.instagram.com/saurabhbahadur_)
+ ### [Discord](https://discord.gg/aQR27Bg7de)


