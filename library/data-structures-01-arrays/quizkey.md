## Data structures: Arrays

1. Recall your solution to the missing-number problem using the brute-force algorithm. Your solution may have looked like this:

    ```
    for i = 1 to n
      if n is not in numbers
         return i
    ```

    What is the running time of this algorithm? 

    **Answer:** D. `O(n^2)`

2. Recall your solution to the missing-number problem using the sum-and-subtract algorithm. Your solution may have looked like this:

    ```
    expectSum = find the sum of all integers from 1 to n
    actualSum = find the sum of all numbers in the array
    return expectedSum - actualSum
    ```

    What is the running time of this algorithm?

    **Answer:** C. `O(n)`

3. After analyzing the two algorithms used to solve the missing-number problem, which of the following should be true?

    **Answer:** B. The sum-and-subtract algorithm is more efficient.

4. Recall your solution to the largest and smallest problem using the sort first algorithm. Your solution may have looked like this:

    ```
    sort the numbers array
    return [numbers[0], numbers[numbers.length - 1]]
    ```

    What is the running time of this algorithm?

    **Answer:** D. `O(n log n)`

5. Recall your solution to the largest and smallest problem using the sort first algorithm. Your solution may have looked like this:

    ```
    largest = negative infinity
    smallest = positive infinity
    for each e in numbers do
      if e is larger than largest
         largest = e
      if e is smaller than smallest
         smallest = e
    return [smallest, largest]
    ```

    What is the running time of this algorithm?

    **Answer:** C. `O(n)`

6. After analyzing the two algorithms used to solve the largest and smallest problem, which of the following should be true?

    **Answer:** A. The iteration algorithm is more efficient.
