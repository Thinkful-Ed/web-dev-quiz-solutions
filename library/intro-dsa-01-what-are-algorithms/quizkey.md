## DSA introduction: What are algorithms?

1. Select all that are true for _computational problems_.

    **Answers:** A, B, D, and F.

    A. Problems must be well-specified.

    B.  The inputs to the problem must be specified.

    D. The outputs of the problem must be specified.

    F. The relationship between the inputs and the outputs must be specified.

2. Select all that are true about _algorithms_.

    **Answers:** A, B, and E.

    A. An algorithm is a solution to a computational problem.

    B. There may be more than one algorithms that solve the same problem.

    E. An algorithm is made up of a finite number of steps. It must stop with a correct output eventually.

3. Consider the following problem:

    Given two integers `a` and `b` as inputs, return the value of `a` divided by `b`. If `b = 0`, return `Cannot divide by zero`.

    The following algorithm purports to solve this problem.

    ```js
    function divide(a, b) {
      return a / b;
    }
    ```
    
    Which property of algorithms does this algorithm _not_ satisfy?
    
    **Answer:** A. Correctness: The output produced by the algorithm is correct for all valid input.

4. The number of steps that are needed to execute an algorithm for a given input is called the...

    **Answer:** B. Time complexity
