# C - Sorting Algorithms & Big O


---

## Description
This project focuses on implementing and understanding various sorting algorithms and analyzing their time complexities using Big O notation.

### Tasks:
- **Implement sorting algorithms**
- **Analyze and optimize their performance**
- **Complete quizzes to test your knowledge**



---

## Data Structure and Functions

### Print Functions
You are provided with the following print functions:

```c
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

These files (`print_array.c` and `print_list.c`) will be compiled alongside your functions during grading. 
Declare their prototypes in `sort.h`.

### Data Structure for Doubly Linked List
```c
/**
 * struct listint_s - Doubly linked list node
 *
 * @n: Integer stored in the node
 * @prev: Pointer to the previous element of the list
 * @next: Pointer to the next element of the list
 */
typedef struct listint_s
{
    const int n;
    struct listint_s *prev;
    struct listint_s *next;
} listint_t;
```

---

## Big O Notation

### Common Notations:
- **O(1):** Constant time.
- **O(n):** Linear time.
- **O(n^2):** Quadratic time.
- **O(log(n)):** Logarithmic time.
- **O(nlog(n)):** Linearithmic time.
- **O(n!):** Factorial time.

When answering quiz questions, use the "short" notation (e.g., `O(nk)` is written as `O(n)`).

---

## Testing

### Tip for Testing Large Inputs
Use [Random.org](https://www.random.org) to generate large sets of random integers for testing your sorting algorithms.

---



---

## Authors
- **Derick Quiñones Medina**


