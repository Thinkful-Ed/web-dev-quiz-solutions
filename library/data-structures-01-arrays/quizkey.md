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
    
    Distractor rationale:  O(N^2) - This is the correct answer because the algorithm iterates over every pair of elements in the array, resulting in a nested loop that runs in quadratic time.

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
    
    Distractor rationale: The correct answer for this question is C. O(N), meaning that the running time of the algorithm grows linearly with the size of the input array.

3. Which of the following statements is true?

A. The findDuplicates algorithm is more efficient than the findLargestNumber algorithm.

B. The findLargestNumber algorithm is more efficient than the findDuplicates algorithm.

C. The running time is about the same for both algorithms.

D. There is no way to tell which is actually better.

    **Answer:** B. The findLargestNumber algorithm is more efficient than the findDuplicates algorithm.
    
    Distractor rationale: The findLargestNumber running time is O(N) whereas the running time of the findDuplicate method is O(N^2). 

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
    
    Distractor rationale: the correct answer of B. O(log N) means that the algorithm's running time increases logarithmically with the size of the input, and the other answer choices can be ruled out based on the characteristics of the algorithm's implementation.


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
    
    Distractor rationale: The correct answer of C. O(N) means that the algorithm's running time increases linearly with the size of the input, and the other answer choices can be ruled out based on the characteristics of the algorithm's implementation.

6. After analyzing the two algorithms used to search for a given element, which of the following should be true?

A. The binarySearch algorithm is more efficient.

B. The linearSearch algorithm is more efficient.

C. They are about the same, so it does not matter.

D. linearSearch uses less lines of code, making it a better choice.

    **Answer:** A. The binarySearch algorithm is more efficient.
    
    Distractor rationale: A running time of O(log n) is more efficient than O(n).
