# Practice Challenge: Stack Plus

In this practice challenge, you will get an opportunity to use the Data
Structures and Algorithms skills you have built over the course of the program.
It will also help you prepare for the types of challenges you can expect to see
in job interviews.

## Instructions

Implement a `StackPlus` class that has the following methods:

- `#push(value)`: Pushes the value (Integer) to the top of the stack
- `#pop`: Pop the top value off the stack and return the value. If no values are
  present, return `-1`.
- `#increment(n)`: Increment the value of the bottom `n` number of elements
  by 1. If there are less than `n` number of elements in the stack, increment
  all elements by 1.

**Note**: the tests will only check the return value of calling the `#pop`
method, so you just need to ensure that the values are correct when they've been
removed from the stack.

**Also note**: there is a solution with O(n) runtime for the `#increment`
method. It is possible to solve with O(1) runtime, but the solution is
significantly more challenging. Good luck!

Example 1:

![Stack Plus example](https://curriculum-content.s3.amazonaws.com/phase-5/phase-5-practice-challenge-stack-plus/stack-plus.png)

```rb
stack = StackPlus.new # stack is empty []
stack.push(2) # stack becomes [2]
stack.push(3) # stack becomes [2, 3]
stack.increment(2) # stack becomes [3, 4], increment the bottom 2 elements
stack.pop # return 4, stack becomes [3]
stack.pop # return 3, stack becomes []
```

Example 2:

```rb
stack = StackPlus.new # stack is empty []
stack.push(1) # stack becomes [1]
stack.push(2) # stack becomes [1, 2]
stack.pop # return 2, stack becomes [1]
stack.push(2) # stack becomes [1, 2]
stack.push(3) # stack becomes [1, 2, 3]
stack.increment(5) # stack becomes [2, 3, 4], since 5 is greater than the number of elements, we increment them all
stack.increment(2) # stack becomes [3, 4, 4], only increment the bottom 2 elements
stack.pop # return 4, stack becomes [3, 4]
stack.pop # return 4, stack becomes [3]
stack.pop # return 3, stack becomes []
stack.pop # return -1, stack remains []
```

Remember the process:

1. Rewrite the problem in your own words
2. Write your own test cases
3. Pseudocode
4. Code
5. Refactor to make it clean and readable
6. Refactor to optimize

Once you have a complete solution, run the test suite using `learn test` as a
final check.

## Check Out the Solution

Several possible approaches for completing this challenge are provided in a
separate lesson. Once your code is working and you have all the tests passing,
be sure to take a look at the example solutions provided. This will give you
exposure to different approaches for solving this challenge, and may also give
you ideas for how you might want to refactor your code to make it better.
