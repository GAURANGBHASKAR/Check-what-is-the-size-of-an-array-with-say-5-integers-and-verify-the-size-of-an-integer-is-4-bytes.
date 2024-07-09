# 1)Check-what-is-the-size-of-an-array-with-say-5-integers-and-verify-the-size-of-an-integer-is-4-bytes.

//The size of an array is calculated as the number of elements multiplied by the size of each element. For an array of 5 integers, if an integer is 4 bytes, the total size would be 5 (elements) * 4 (bytes per integer) = 20 bytes.
//To verify the size of an integer we use the "sizeof" operator.
//Code to Verify:-
#include <stdio.h>

int main() {
    printf("Size of an integer: %ld bytes\n", sizeof(int));
    return 0;
}

# 2)Print the address of all the elements in an array of 5 integers.

#include <stdio.h>

int main() {
    int array[5] = {1, 2, 3, 4, 5};
    int i;

    for (i = 0; i < 5; i++) {
        printf("Address of array[%d]: %p\n", i, &array[i]);
    }

    return 0;
}

