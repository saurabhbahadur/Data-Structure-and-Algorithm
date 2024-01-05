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

### Reversal in An Array

```java
public class demo {
    public static void main(String[] args) {
        int arr[] = { 1, 2, 3, 4, 5 };
        int n = arr.length;
        for (int i = 0; i < n / 2; i++) {
            int temp = arr[i];
            arr[i] = arr[n - i - 1];
            arr[n - i - 1] = temp;
        }

        for (int i = 0; i < n; i++) {
            System.out.println(arr[i]);
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


