<h1 align="center"> Searching In Arrays   </h1>
<p align="center" > () </p>

### Searching  in Array
+ Linear Search
+ Binary Search

### 1. Linear Search
+ It is simple and straight forward search algorithm used to find a specific element within an array or list

#### Advantages
+ Simple to understand
+ It is used in both `sorted` and `unsorted` array.
+ No additional memory

#### Disadvantages
+ When n is big then there time complexity is high

```java
public class demo {
    public static int linearSearch(int num[], int target) {
        for (int i = 0; i <= num.length; i++) {
            if (num[i] == target) {
                return i;
            }
        }
        return -1;
    }

    public static void main(String[] args) {
        int num[] = { 1, 3, 5, 6, 8, 9 };
        int target = 6;

        int idx = linearSearch(num, target);
        if (idx == -1) {
            System.out.println("Target value not found");

        } else {
            System.out.println("Target value found  " + idx);
        }
    }
}

```

```java
import java.util.Scanner;

public class demo {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter number of element you want to enter");
        int n = sc.nextInt();

        System.out.println("Enter " + n + " element for array ");
        int arr[] = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        System.out.println("Enter the target value you want to search");
        int target = sc.nextInt();
        int idx = -1;

        // Implementation of Linear Search
        for (int i = 0; i < n; i++) {
            if (arr[i] == target) {
                idx = i;
                break;
            }
        }

        if (idx == -1) {
            System.out.println("Target Value not found");
        } else {
            System.out.println("Target value found at index:  " + idx);
        }

    }
}
```

### 2. Binary Search
+ It is an efficient search algorithm used to find a specific element within a `sorted` array or list.
+ It works by repeteadely dividing the search interval in half and comparing the middle element with the target value.

#### Advantages
+ Low in Time Complexity [O(Log n)].

#### Disadvantages
+ We have to use Binary Search in Sorted Array

```java
public class demo {
    public static int binarySearch(int num[], int target) {
        int start = 0;
        int end = num.length - 1;

        while (start <= end) {
            int mid = start + (end - start) / 2;
            if (num[mid] == target) {
                return mid;
            } else if (num[mid] > target) {
                end = mid - 1;
            } else if (num[mid] < target) {
                start = mid + 1;
            }
        }
        return -1;
    }

    public static void main(String[] args) {
        int num[] = { 1, 3, 5, 6, 8, 9 };
        int target = 9;

        int idx = binarySearch(num, target);
        if (idx == -1) {
            System.out.println("Target value not found");

        } else {
            System.out.println("Target value found  " + idx);
        }
    }
}

```

```java
import java.util.Scanner;

public class demo {

    public static int binarySearch(int[] arr, int target) {
        int low = 0;
        int high = arr.length - 1;

        while (low <= high) {
            int mid = low + (high - low) / 2;
            if (arr[mid] == target) {
                return mid;
            } else if (arr[mid] < target) {
                low = mid + 1;
            } else {
                high = mid - 1;
            }
        }
        return 0;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter number of element you want to enter");
        int n = sc.nextInt();

        System.out.println("Enter " + n + " element for array ");
        int arr[] = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        System.out.println("Enter the target value you want to search");
        int target = sc.nextInt();

        // Implementation of Binary Search
        int result = binarySearch(arr, target);

        if (result == 0) {
            System.out.println("Target Value not found");
        } else {
            System.out.println("Target value found at index:  " + result);
        }

    }
}

```

### Interview Problem:  Lower Bound/ First occurence of an element
```java
import java.util.Scanner;

public class demo {

    public static int findFirstOccurence(int[] arr, int target) {
        int low = 0;
        int high = arr.length - 1;
        int result = -1;

        while (low <= high) {
            int mid = low + (high - low) / 2;
            if (arr[mid] == target) {
                result = mid;
                high = mid - 1;
            } else if (arr[mid] > target) {
                high = mid - 1;
            } else {
                low = mid + 1;
            }
        }
        return result;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.println("Please enter number of element you want to enter");
        int n = sc.nextInt();

        System.out.println("Enter " + n + " element for array ");
        int arr[] = new int[n];

        for (int i = 0; i < n; i++) {
            arr[i] = sc.nextInt();
        }

        System.out.println("Enter the target value you want to search");
        int target = sc.nextInt();

        // Implementation
        int result = findFirstOccurence(arr, target);

        if (result == -1) {
            System.out.println("Target Value not found");
        } else {
            System.out.println("Target value found at index:  " + result);
        }

    }
}

```
### Interview Problem: Square Root

```java



```

***

# Feel Free to connect
+ ### [LinkedIn](https://www.linkedin.com/in/saurabhbahadur)
+ ### [Mail](mailto:singhsaurabhbahadur@gmail.com)
+ ### [Instagram](https://www.instagram.com/saurabhbahadur_)
+ ### [Discord](https://discord.gg/aQR27Bg7de)


