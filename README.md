# Animated Sorting of an Array
A visualization for a bunch of different sorting algorithms in Javascript.

More specifically, we visualize in-place comparison-based sorting algorithms by highlighting each comparison in blue and each swap in red. Currently the following sorting algorithms are implemented:

* [Bubble sort](https://en.wikipedia.org/wiki/Bubble_sort)
* [Insertion sort](https://en.wikipedia.org/wiki/Insertion_sort)
* [Quicksort](https://en.wikipedia.org/wiki/Quicksort)
* [Heapsort](https://en.wikipedia.org/wiki/Heapsort)
* [Merge sort](https://en.wikipedia.org/wiki/Merge_sort)

Quicksort recursively partition chunks of the array around a pivot value; the choice of pivot can have a big effect on the efficiency of the algorithm. We implement several pivoting choices discussed [here](https://en.wikipedia.org/wiki/Quicksort#Choice_of_pivot).

The current mergesort implementation isn't *really* in-place; during the merge step, we scan the sorted subarrays to build up a permutation that will merge them, then convert the permutation to a sequence of swaps. These intermediate data structures use a linear amount of extra memory.

