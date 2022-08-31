# codecademy-divide_and_conquer_algorithms


Divide and Conquer in Three Steps

The divide-and-conquer strategy is a three-step process:

Divide: Recursively divide a big problem into smaller subproblems.
Conquer: Solve the subproblems after they become small enough.
Combine: Merge the subproblems to get the desired solution.
This process might look familiar to you because it is the principle behind merge sort. Let us review merge sort and understand how it utilizes divide-and-conquer to efficiently sort an array.

The given array to be sorted is: 

Divide

First, we need to divide into smaller subproblems. In merge sort, the array is split into two halves in each step. After the first step, the array will look like this: 

But wait, the subproblems are still not small enough to be solved. We need to recursively divide the problem until every subarray only contains one number: third-divide At this point, the subproblems are considered solved on their own because an array consisting of only one number is sorted.

Conquer & Combine

Now it’s time to combine the subproblems together. “Conquer” will work side by side with “combine” in the following steps, in the sense that we need to merge two subarrays in the correct order.

After all the subproblems are combined, we get the sorted array as the result. complete
Multiple choice
Suppose you are tasked to analyze a spreadsheet consisting of 80 entries. You decide to use a divide-and-conquer approach and divide the problem into two equal halves in each step. How many entries will each subproblem have after three steps of division?

10

5

8

13

Time & Space Complexities

There is no single time or space complexity that can describe all divide-and-conquer algorithms. However, we can follow these general rules to determine the big-O runtime of a specific algorithm:

Because the problem is divided into at least 2 subproblems at each step, the number of steps needed to divide the problem is log(n).
The cost of solving and merging the subproblems is a factor as well. This is often multiplied by the cost of division to get the overall runtime.
For merge sort, division takes O(log(n)) time, and combining the sorted sublists takes O(n) time. Therefore, merge sort has a big-O runtime of O(nlog(n)).

The space complexity also varies from algorithm to algorithm. Divide-and-conquer usually requires more space than other paradigms due to the overhead of the recursion stack.

Pros and Cons

Divide-and-conquer has several advantages:

It let us solve conceptually complex problems by breaking them into smaller subproblems.
It has a better asymptotic cost than brute force approaches and is used in many efficient algorithms such as merge sort and quicksort.
It makes efficient use of memory caches, which are the fastest type of memory units in a computer.
However, it does have some issues as well:

Since divide-and-conquer algorithms are usually implemented recursively, they require additional memory allocation on the stack. If a divide-and-conquer algorithm is executed without sufficient memory, a stack overflow error will occur.
Divide-and-conquer cannot avoid evaluating the same subproblem repeatedly, making it a bad fit for problems that have overlapping subproblems.
Multiple choice
Which of the following statements about divide-and-conquer is NOT true?

Divide-and-conquer should not be used for problems that produce many overlapping subproblems.

Divide-and-conquer algorithms are usually recursive.

Divide-and-conquer algorithms are more efficient than brute force algorithms.

Divide-and-conquer algorithms can run very well on systems with small memory.
Review

Good job! You have learned a lot about divide-and-conquer algorithms!

Let’s review what we covered:

Divide-and-conquer is a strategy that solves a large problem by recursively breaking it down into smaller subproblems until they can be solved directly.
Divide-and-conquer works in three steps: divide, conquer, and combine.
The time complexity of a divide-and-conquer algorithm is determined by the cost of division (log(n)) and the cost of solving the subproblems.
Advantages:
Simplify large and complex problems by breaking them down into subproblems.
More efficient than brute force approaches.
Can access memory caches efficiently.
Disadvantages:
Risk of stack overflow due to the recursion stack.
Cannot avoid evaluating the same subproblem repeatedly.
Back
