## DSA introduction: Some common functions

1. Here are four functions that are commonly used to describe the growth of algorithms. Rank these functions from best (slowest growth) to worst (fastest growth).

    **Answer:** C. c, d, b, a

2. Which kind of growth best characterizes the function `7n`?

    **Answer:** B. Linear

3. Which kind of growth best characterizes the function `2000`?

    **Answer:** A. Constant

4. Which kind of growth best characterizes the function `3^n`?

    **Answer:** D. Exponential

5. Which kind of growth best characterizes the function `2 log n`?

    **Answer:** C. Logarithmic

6. Which of the following functions has the same growth rate as the graph?

    **Answer:** B. `13n+3`

7. What is the order of growth of the following function?

    ```js
    function sumDistinct(numbers) {
      //accepts: numbers - an array of integers
      let highest = Number.NEGATIVE_INFINITY;
      for(let i = 0; i < numbers.length; i++) {
        let sum = 0;
        for(let j = i; j < numbers.length; j++) {
          if(numbers[j] === numbers[i]) {
            sum += numbers[i];
          }
        }
        if(sum > highest) {
          highest = sum;
        }
      }
      return highest;
    }
    ```

    **Answer:** B. `O(n^2)`
