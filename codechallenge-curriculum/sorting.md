# Sorting
---wip---

---

## O(n^2)

### Bubble Sort
```python
def bubbleSort(arr):
    n = len(arr)

    # Traverse through all array elements
    for i in range(n):
        swapped = False

        # Last i elements are already in place
        for j in range(0, n-i-1):

            # Traverse the array from 0 to n-i-1
            # Swap if the element found is greater
            # than the next element
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
                swapped = True
        if (swapped == False):
            break

# Driver code to test
bubbleSort(arr)
print("Sorted array:")
for i in range(len(arr)):
    print("%d" % arr [i], end=" ")
```

### Insertion Sort

### Selection Sort

## O(nlog(n))

### Quicksort

### Mergesort

### Timsort

### Heapsort

## O(n+k)

### Bucket Sort

### Radix Sort

### Counting Sort