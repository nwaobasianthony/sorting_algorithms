# 0x1B. C - Sorting algorithms & Big O

![CFYYWy6UEAE9Ow-](https://s3.amazonaws.com/intranet-projects-files/holbertonschool-low_level_programming/248/willy-wonka.png)

## Resources
**Read or watch:**

* Sorting algorithm
* Big O notation
* Sorting algorithms animations
* 15 sorting algorithms in 6 minutes (WARNING: The following video can trigger seizure/epilepsy. It is not required for the project, as it is only a funny visualization of different sorting algorithms)
* CS50 Algorithms explanation in detail by David Malan
* All about sorting algorithms

## Requirements
### General

* Allowed editors: `vi`, `vim`, `emacs`
* All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options `-Wall -Werror -Wextra -pedantic -std=gnu89`
* All your files should end with a new line
* A `README.md` file, at the root of the folder of the project is mandatory
* Your code should use the `Betty` style. It will be checked using [betty-style.pl]() and [betty-doc.pl]()
* You are not allowed to use global variables
* No more than 5 functions per file

* Unless specified otherwise, you are not allowed to use the standard library. Any use of functions like printf, puts, … is totally forbidden.
* In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples
* The prototypes of all your functions should be included in your header file called `sort.h`
* Don’t forget to push your header file
* All your header files should be include guarded
* A list/array does not need to be sorted if its size is less than 2.

## More Info
### Data structures

* For this project you are given the following `print_array`, and `print_list` functions:

```
#include <stdlib.h>
#include <stdio.h>

/**
 * print_array - Prints an array of integers
 *
 * @array: The array to be printed
 * @size: Number of elements in @array
 */
void print_array(const int *array, size_t size)
{
    size_t i;

    i = 0;
    while (array && i < size)
    {
        if (i > 0)
            printf(", ");
        printf("%d", array[i]);
        ++i;
    }
    printf("\n");
}
```

```
#include <stdio.h>
#include "sort.h"

/**
 * print_list - Prints a list of integers
 *
 * @list: The list to be printed
 */
void print_list(const listint_t *list)
{
    int i;

    i = 0;
    while (list)
    {
        if (i > 0)
            printf(", ");
        printf("%d", list->n);
        ++i;
        list = list->next;
    }
    printf("\n");
}
```


## Tasks
[0 - Bubble sort](./0-bubble_sort.c)
[1 - Insertion sort](./1-insertion_sort_list.c)
[2 - Selection sort](./2-selection_sort.c)
[3 - Quick sort](./3-quick_sort.c)
[4 - Shell sort](./100-shell_sort.c)
[5 - Cocktail shaker sort](./101-cocktail_sort_list.c)
[6 - Quick sort](./102-counting_sort.c)
[7 - Merge sort](./103-merge_sort.c)
[8 - Heap sort](./104-heap_sort.c)
[9 - Radix sort](./105-radix_sort.c)
[10 - Bitonic sort](./106-bitonic_sort.c)
[11 - Quick sort](./107-quick_sort_hoare.c)
