<h1 align="center"> Sorting In Arrays   </h1>
<p align="center" > (
Compare, swap, repeat, until sorted) </p>

### Sorting  in Array
+ Sorting an array means to arrange the elements in the array in a certain order.
+ Some Algorithm we choose to sort are:
    + Bubble Sort
    + Insertion Sort
    + Selection Sort

### Bubble Sort
+ Bubble Sort is a simple sorting algorithm.
+ This sorting algorithm is comparison-based algorithm in which each pair of adjacent element is compared and the element are swapped if they are not in order. 

```java
import java.util.Arrays;

public class demo {

    public static void bubbleSort(int arr[]) {
        for (int i = 0; i < arr.length; i++) {
            boolean swapped = false;
            for (int j = 0; j < arr.length - i - 1; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                    swapped = true;
                }

            }
            if (!swapped) {
                break;
            }
        }
    }

    public static void main(String[] args) {
        int arr[] = { 1, 83, 77, 45, 19, 8 };

        bubbleSort(arr);

        System.out.println(Arrays.toString((arr)));

    }
}
```
```java
public class demo {

    public static void bubbleSort(int arr[]) {
        for (int i = 0; i < arr.length; i++) {
            for (int j = 0; j < arr.length - i - 1; j++) {
                if (arr[j] > arr[j + 1]) {
                    int temp = arr[j];
                    arr[j] = arr[j + 1];
                    arr[j + 1] = temp;
                }
            }
        }
    }

    public static void printArray(int arr[]) {
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i]);
        }
    }

    public static void main(String[] args) {
        int arr[] = { 1, 8, 2, 7, 9, 10 };
        bubbleSort(arr);
        printArray(arr);

    }
}

```


### Insertion Sort
+ It is a simple sorting algorithm that works similar to the way you sort playing cards in your hands.

```java
import java.util.Arrays;

public class demo {

    public static void insertionSort(int arr[]) {
        for (int i = 1; i < arr.length; i++) {
            int j = i;
            while (j > 0 && arr[j] < arr[j - 1]) {
                int temp = arr[j];
                arr[j] = arr[j - 1];
                arr[j - 1] = temp;
                j--;
            }
        }
    }

    public static void main(String[] args) {
        int arr[] = { 1, 83, 77, 45, 19, 8 };

        insertionSort(arr);

        System.out.println(Arrays.toString((arr)));

    }
}
  

```

### Selection Sort
+ It is a simple and efficient sorting algorithm that works by repeatedly selecting the smallest element form the unsorted portion of the list and moving it to the sorted portion of the list. 

```java
import java.util.Arrays;

public class demo {

    public static void selectionSort(int arr[]) {
        for (int i = 0; i < arr.length; i++) {
            int min_idx = i;
            for (int j = i + 1; j < arr.length; j++) {
                if (arr[j] < arr[min_idx]) {
                    min_idx = j;
                }
            }
            if (min_idx != i) {
                int temp = arr[min_idx];
                arr[min_idx] = arr[i];
                arr[i] = temp;
            }
        }
    }

    public static void main(String[] args) {
        int arr[] = { 1, 83, 77, 45, 19, 8 };

        selectionSort(arr);

        System.out.println(Arrays.toString((arr)));

    }
}
```

```java
public class demo {
    public static void selectionSort(int arr[]) {
        for (int i = 0; i < arr.length - 1; i++) {
            int min_pos = i;
            for (int j = i + 1; j < arr.length; j++) {
                if (arr[min_pos] > arr[j]) {
                    min_pos = j;
                }
            }
            int temp = arr[min_pos];
            arr[min_pos] = arr[i];
            arr[i] = temp;
        }
    }
    public static void printArray(int arr[]) {
        for (int i = 0; i < arr.length; i++) {
            System.out.print(arr[i]);
        }
    }

    public static void main(String[] args) {
        int arr[] = { 1, 8, 2, 7, 9, 10 };
        selectionSort(arr);
        printArray(arr);

    }
}


```
 






---

<h3 align="center">Connect with me:</h3>
<p align="center">
<a href="https://twitter.com/saurabhbahadur" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/twitter.svg" alt="saurabhbahadur" height="30" width="40" /></a>
<a href="https://linkedin.com/in/saurabhbahadur" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/linked-in-alt.svg" alt="saurabhbahadur" height="30" width="40" /></a>
<a href="https://fb.com/singhsaurabhbahadur" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/facebook.svg" alt="singhsaurabhbahadur" height="30" width="40" /></a>
<a href="https://instagram.com/saurabhbahadur_" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/instagram.svg" alt="saurabhbahadur_" height="30" width="40" /></a>
<a href="https://www.youtube.com/c/mighty saur" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/youtube.svg" alt="mighty saur" height="30" width="40" /></a>
<a href="https://www.hackerrank.com/saurabhbahadur" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/hackerrank.svg" alt="saurabhbahadur" height="30" width="40" /></a>
<a href="https://discord.gg/aQR27Bg7de" target="blank"><img align="center" src="https://raw.githubusercontent.com/rahuldkjain/github-profile-readme-generator/master/src/images/icons/Social/discord.svg" alt="aQR27Bg7de" height="30" width="40" /></a>
</p>

---
