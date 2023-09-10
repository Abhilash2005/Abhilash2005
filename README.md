def selection_sort(arr):
    n = len(arr)
    for i in range(n):
        # Assume the current index is the minimum
        min_index = i
        
        Find the minimum element in the remaining unsorted part
        for j in range(i + 1, n):
            if arr[j] < arr[min_index]:
                min_index = j
                
         Swap the found minimum element with the first element of the unsorted part
        arr[i], arr[min_index] = arr[min_index], arr[i]
        
 Sample input list
input_list = [64, 34, 25, 12, 22, 11, 90]

print("Input List:", input_list)

 Perform selection sort on the input list
selection_sort(input_list)

print("Sorted List:", input_list)
