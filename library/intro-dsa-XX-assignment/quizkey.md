## DSA introduction: Assessment

### Greatest common divisor (GCD) problem

The GCD of two positive integers `a` and `b` is the largest of the common divisors of `a` and `b`. If a number `c` can be divided by another number `d` without leaving a remainder, it's said that `d` is a divisor of `c`.

For example, the GCD of `24` and `30` is `6`, because the divisors of 24 are 1, 2, 3, 4, 6, 8, 12, and 24, and the divisors of `30` are 1, 2, 3, 5, 6, 10, 15, and 30.

The common divisors of `24` and `30` are 1, 2, 3, and 6. And `6` is the largest of these common divisors.

Below are two algorithms for solving the GCD problem. Review them carefully:

#### Algorithm 1

This algorithm was developed by Euclid (circa 300 B.C.).

```js
function gcd1(a, b) {
  // if a is equal to 0 then the GCD of a and b is b, so return b
  if (a === 0) {
    return b;
  }

  // if b is equal to 0 then the GCD of a and b is a, so return a
  if (b === 0) {
    return a;
  }

  while (b !== 0) {
    // let r be the remainder of dividing a by b
    const r = a % b;
    a = b;
    b = r;
  }

  return a;
}
```

#### Algorithm 2

This is a brute-force approach to solving the GCD problem. It iterates over all the divisors of both `a` and `b` and finds the common ones then finds the largest.

```js
function gcd2(a, b) {
  if (a === 0) {
    return b;
  }

  if (b === 0) {
    return a;
  }

  const divA = [1, a];
  const divB = [1, b];
  const common = [];

  for (let i = 2; i < a; i++) {
    if (a % i === 0) {
      divA.push(i);
    }
  }

  for (let i = 2; i < b; i++) {
    if (b % i === 0) {
      divB.push(i);
    }
  }

  for (let i = 0; i < divA.length; i++) {
    if (divB.includes(divA[i])) {
      common.push(divA[i]);
    }
  }

  let largest = Number.NEGATIVE_INFINITY;
  for (let i = 0; i < common.length; i++) {
    if (common[i] > largest) {
      largest = common[i];
    }
  }

  return largest;
}
```

Please answer the following questions related to the GCD algorithms described above.

#### Algorithm 1

1. After running algorithm 1 a few times, the following table of running times was constructed.

| n         | time in nanoseconds |
| --------- | ------------------- |
| 1,000     | 2177                |
| 100, 000  | 2344                |
| 1,000,000 | 2742                |

Which of the following represents the most likely growth rate of this algorithm?

A. O(n)
B. O(log n)
C. O(n^2)
D. None of the above

**Answer:** B. `O(log n)`
**Distractor Rationale:** Algorithm 1 has a logarithmic time complexity of O(log n) because it halves the size of the input with each iteration in the while loop.

2. Which of the following graphs is most likely to depict the growth rate of algorithm 1?

A.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/0240465175d05b84928d56de446fc731-image.png)

B.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/f5691d14e18dc8982919069045efb69c-image.png)

C.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/923e7973e77d3db906e98892d6df6005-image.png)

D. None of the above

**Answer:** A
**Distractor Rationale:** Algorithm 1 has a logarithmic time complexity of O(log n) because it halves the size of the input with each iteration in the while loop. The graph in option A depicts a logarithmic growth rate where the running time increases very slowly as the input size increases. Option B depicts a linear growth rate where the running time increases linearly as the input size increases. Algorithm 1 does not have a linear time complexity. Option C depicts an exponential growth rate where the running time increases very rapidly as the input size increases. Algorithm 1 does not have an exponential time complexity.

#### Algorithm 2

3. After running algorithm 2 a few times, the following table of running times was constructed.

| n         | time in nanoseconds |
| --------- | ------------------- |
| 1,000     | 126,168             |
| 100, 000  | 12,526,036          |
| 1,000,000 | 71,130,340          |

Which of the following represents the most likely growth rate of this algorithm?

A. O(n)
B. O(log n)
C. O(n^2)
D. None of the above

**Answer:** A. `O(n)`
**Distractor Rationale:** Algorithm 2 has a linear time complexity of O(n) because it iterates over all the divisors of both input numbers, which is proportional to the input size.

4. Which of the following graphs is most likely to depict the growth rate of algorithm 2?

A.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/0240465175d05b84928d56de446fc731-image.png)

B.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/f5691d14e18dc8982919069045efb69c-image.png)

C.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/923e7973e77d3db906e98892d6df6005-image.png)

D. None of the above

**Answer:** B
**Distractor Rationale:** Algorithm 2 has a linear time complexity of O(n) because it iterates over all the divisors of both input numbers, which is proportional to the input size. The graph in option B depicts a linear growth rate where the running time increases linearly as the input size increases.

5. Review algorithm 2.

```
function gcd2
  // accepts a - a non-negative integer
  //         b - a non-negative integer

  if a is equal to 0 then the GCD of a and b is b, so return b
  if b is equal to 0 then the GCD of a and b is a, so return a

  initialize an array named divA with the value [1, a] //<== A
  initialize an array named divB with the value [1, b]
  initialize an empty array named common

  for i = 2 to a - 1 do  //<== B
    if a can be divided by i without a remainder then
      add i to the array divA

  for i = 2 to b - 1 do
    if b can be divided by i without a remainder then
      add i to the array divB

  for each number n in the array divA do:
    if n is in the array divB then
       add n to the array common

  initialize a variable named largest to the smallest possible number
  for each number n in commmon do:
    if n is greater than largest then
      assign largest the value n

  return largest
```

Notice the lines marked A and B. Which of the following statements are true?

A. A runs once `O(1)`, and B runs `a-3` times `O(a)`.

B. A runs once `O(1)`, and B runs once `O(1)`.

C. A runs once for each element in the `divA` array, and B runs once for each element of the `divB` array.

**Answer:** A. A runs once `O(1)`, and B runs `a-3` times `O(a)`.
**Distractor Rationale:** The algorithm initializes the `divA` array with the value `[1, a]` and then loops through `a-2` elements to find all the divisors of `a`. This means that the for loop runs `a-3` times, which results in a time complexity of `O(a)` for this section of the algorithm. On the other hand, the initialization of the `divA` array in line A only runs once, which results in a time complexity of `O(1)`. Therefore, statement A is true.

### Split sum problem

You have been asked to help organize tours for groups of school children to view the Butterfly Pavilion at the museum. To your surprise, the exhibit is quite popular, and many groups have registered an interest in the tour.

You decide that you will have to hold the tours across two days to accommodate the groups. You need to select a number of groups to visit on the first day and a number of groups to visit on the second day, such that each day has roughly the same number of visitors.

You have the sizes of each group recorded in an array. You wish to select the point at which to split the array so that the difference between the sums of each part of the array is minimum.

For example, suppose the following array of group sizes was given.

[4, 12, 17, 8, 13, 24, 9]

If you split at index `2`, the first part of the array contains `4`, `12`, and `17`, giving the sum `33`. The second part of the array contains the numbers `8`, `13`, `24`, and `9`, giving the sum `54`. The difference is `54 - 33 = 21`.

However, if you split at index `3`, the first part of the array contains `4`, `12`, `17`, and `8`, giving the sum `41`, and the second part of the array contains `13`, `24`, and `9`, giving the sum `46`. The difference here is `46 - 41 = 5`.

The objective of the split sum problem is to find the smallest possible difference over all splits.

Below are two algorithms for solving the Split Sum problem. Review them carefully:

#### Algorithm 1

This algorithm works by first finding the sum of the whole array then iterating through the array. At each position `i` in the array, the sum from `0` to `i` is calculated from the total sum, and the sum from `i+1` to the end of the array is calculated from the total sum. These two sums are compared.

```js
function splitSum1(tours) {
  // find the sum of the whole array
  const total = tours.reduce((a, c) => a + c, 0); // O(n)

  let preSum = 0;
  let postSum = total;
  let smallest = Number.POSITIVE_INFINITY;

  // for loop goes from second element to second-to-last element
  for (let i = 0; i < tours.length - 1; i++) {
    preSum = preSum + tours[i];
    postSum = postSum - tours[i];

    const difference = Math.abs(preSum - postSum);
    if (difference < smallest) {
      smallest = difference;
    }
  }
  return smallest;
}
```

#### Algorithm 2

This algorithm once again iterates through the array of numbers. At each position `i` in the array, the sum of the numbers from position `0` to `i` is calculated, and the sum of the numbers from i+1 to the end of the array is calculated. The difference is found and compared to the smallest number so far.

```js
let smallest = Number.POSITIVE_INFINITY;
for (let k = 0; k < tours.length; k++) {
  let preSum = tours.slice(0, k + 1).reduce((a, c) => a + c, 0);
  let postSum = tours.slice(k + 1).reduce((a, c) => a + c, 0);
  const difference = Math.abs(preSum - postSum);
  if (difference < smallest) {
    smallest = difference;
  }
}
return smallest;
```

Please answer the following questions related to the Split Sum algorithms presented above.

#### Algorithm 1

1. After running the algorithm several times, the following times were noted.

| n      | Time in nanoseconds |
| ------ | ------------------- |
| 100    | 67,077              |
| 1,000  | 654,726             |
| 10,000 | 7,547,788           |

Which of the following represents the most likely growth rate of this algorithm?

A. `O(1)`
B. `O(n)`
C. `O(n log n)`
D. `O(n^2)`

**Answer:** B. `O(n)`
**Distractor Rationale:** Option B aligns well with the data provided, where the time taken appears to increase proportionally with the input size. Therefore, this is the most likely growth rate of the algorithm.

2. Which of the following graphs is most likely to depict the growth rate of algorithm 1?

A.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/0240465175d05b84928d56de446fc731-image.png)

B.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/f5691d14e18dc8982919069045efb69c-image.png)

C.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/923e7973e77d3db906e98892d6df6005-image.png)

D. None of the above

**Answer:** B
**Distractor Rationale:** Algorithm 1 has a linear time complexity of O(n) because it iterates over the list of tours, which is proportional to the input size.

#### Algorithm 2

3. After running the algorithm several times, the following times were noted.

| n      | time in nanoseconds |
| ------ | ------------------- |
| 100    | 446,609             |
| 1,000  | 35,332,527          |
| 10,000 | 830,602,845         |

Which of the following represents the most likely growth rate of this algorithm?

A. `O(1)`
B. `O(n)`
C. `O(n log n)`
D. `O(n^2)`

**Answer:** D. `O(n^2)`
**Distractor Rationale:** The given times increase much more rapidly than linearly or quasilinearly with larger input sizes.

4. Which of the following graphs is most likely to depict the growth rate of algorithm 2?

A.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/0240465175d05b84928d56de446fc731-image.png)

B.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/f5691d14e18dc8982919069045efb69c-image.png)

C.

![image.png](//res.cloudinary.com/strive/image/upload/w_1000,h_1000,c_limit/923e7973e77d3db906e98892d6df6005-image.png)

D. None of the above

**Answer:** C
**Distractor Rationale:** Option C depicts a graph that exhibits quadratic time complexity.

5. Select the statements that are true.

A. Algorithm 1 is a more efficient algorithm than algorithm 2.

B. It is not possible to say which algorithm is more efficient.

C. Even though the algorithms have different growth rates, it does not matter for very large inputs.

**Answer:** A. Algorithm 1 is a more efficient algorithm than algorithm 2.
**Distractor Rationale:** Statement B is false, as the growth rates of the algorithms are provided, so it is possible to determine which algorithm is more efficient. Statement C is false, as the growth rate of an algorithm becomes increasingly important as input size increases.
