## Data structures: Arrays

1. Consider the following function:

```js
function findDuplicates(arr) {
  let duplicates = [];
  for (let i = 0; i < arr.length; i++) {
    for (let j = i + 1; j < arr.length; j++) {
      if (arr[i] === arr[j] && !duplicates.includes(arr[i])) {
        duplicates.push(arr[i]);
      }
    }
  }
  return duplicates;
}
```
What is the running time of this algorithm?

A. O(1)

B. O(log N)

C. O(N)

D. O(N^2)

    **Answer:** D. `O(N^2)`

2. Consider the following function:

```js
function findLargestNumber(numbers) {
  let max = numbers[0];
  for (let i = 1; i < numbers.length; i++) {
    if (numbers[i] > max) {
      max = numbers[i];
    }
  }
  return max;
}
```
What is the running time of this algorithm?

A. O(1)

B. O(log N)

C. O(N)

D. O(N^2)

    **Answer:** C. `O(N)`

3. Which of the following statements is true?

A. The findDuplicates algorithm is more efficient than the findLargestNumber algorithm.

B. The findLargestNumber algorithm is more efficient than the findDuplicates algorithm.

C. The running time is about the same for both algorithms.

D. There is no way to tell which is actually better.

    **Answer:** B. The findLargestNumber algorithm is more efficient than the findDuplicates algorithm.

4. Consider the following function:

```js
function binarySearch(numbers, target) {
  let left = 0;
  let right = numbers.length - 1;
  while (left <= right) {
    let mid = Math.floor((left + right) / 2);
    if (numbers[mid] === target) {
      return mid;
    } else if (numbers[mid] < target) {
      left = mid + 1;
    } else {
      right = mid - 1;
    }
  }
  return -1;
}
```
What is the running time of this algorithm?

A. O(1)

B. O(log N)

C. O(N)

D. O(N^2)

    **Answer:** B. O(log N)


5. Consider the following function:

```js
function linearSearch(numbers, target) {
  for (let i = 0; i < numbers.length; i++) {
    if (numbers[i] === target) {
      return i;
    }
  }
  return -1;
}
```
What is the running time of this algorithm?

A. O(1)

B. O(log N)

C. O(N)

D. O(N^2)

    **Answer:** C. `O(N)`

6. After analyzing the two algorithms used to search for a given element, which of the following should be true?

A. The binarySearch algorithm is more efficient.

B. The linearSearch algorithm is more efficient.

C. They are about the same, so it does not matter.

D. linearSearch uses less lines of code, making it a better choice.

    **Answer:** A. The binarySearch algorithm is more efficient.
