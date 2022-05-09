## Space complexity problems

1. What is the space complexity of the following algorithm?

    ```js
    function calculateAverageScore(scoresArray){
      let total = 0;
      for(const score of scoresArray){
        total += score
      }
      return total/scoresArray.length
    }
    ```

    **Answer:** C. `O(n)`

2. What is the space complexity of an algorithm?

    **Answer:** B. The maximum working storage an algorithm needs in memory

3. What is the space complexity of the `quickSort` algorithm?

    **Answer:** B. `O(log n)`

4. What is the relationship between space complexity and time complexity?

    **Answer:** D. Space and time complexity are usually correlated.
