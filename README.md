

Preview

Code

---- EXPERIMENT 1 — Stack ADT : ---- Q1. What is an Abstract Data Type (ADT)? An Abstract Data Type (ADT) is a logical description of a data structure that defines the operations that can be performed and the behaviour of those operations, without specifying how they are implemented. It focuses on functionality rather than implementation. Example: Stack ADT defines push, pop, and peek operations.
Q2. Why are push and pop operations O(1)? Push and pop operate only on the top element of the stack and they do not require traversal or shifting of elements . Hence, the number of steps required is constant and independent of stack size. Hence, time complexity = O(1).
Q3. Give one real-world use of stack. A stack is used in function call management in programming languages . Each function call is stored in the call stack, and when the function finishes, it is removed in Last-In-First-Out order.
---- EXPERIMENT 2 — Complexity Analysis : ---- Q1. What is the difference between Big-O and Big-Theta notation? Big-O notation represents the upper bound of algorithm growth, usually describing worst-case complexity. Big-Theta notation represents the exact asymptotic growth rate, meaning both upper and lower bounds are the same.
Q2. What does worst-case complexity represent? Worst-case complexity represents the maximum number of operations an algorithm performs for any input of size n. It shows the slowest possible performance.
Q3. Why is complexity analysis important in real systems? Complexity analysis helps in: selecting efficient algorithms predicting performance for large inputs reducing execution time and memory usage building scalable software systems
---- EXPERIMENT 3 — Recursive Factorial : ---- Q1. What is recursion depth? Recursion depth is the maximum number of recursive function calls present in the call stack simultaneously during execution.
Q2. Why does recursion use stack memory? Each recursive call requires memory to store: function parameters local variables return address These are stored in the call stack until execution completes.
Q3. When is iteration preferred over recursion? Iteration is preferred when: recursion depth is large stack memory is limited performance overhead of function calls must be avoided .
---- EXPERIMENT 4 — Fibonacci : ---- Q1. Why is naive recursive Fibonacci inefficient? Naive recursion repeatedly calculates the same Fibonacci values multiple times, leading to redundant computations. This causes exponential growth in function calls.
Q2. How is memoization related to dynamic programming? Memoization is a technique used in dynamic programming where results of previously solved subproblems are stored and reused. This avoids repeated computation and improves efficiency.
Q3. What is the space impact of memoization? Memoization requires additional memory to store computed values. Therefore, extra space complexity is O(n).
---- EXPERIMENT 5 — Tower of Hanoi ---- Q1. Why is the number of moves equal to 2ⁿ − 1? To move n disks: move n−1 disks to auxiliary rod move largest disk move n−1 disks again This gives recurrence: T(n) = 2T(n−1) + 1 Solving gives 2ⁿ − 1 moves.
Q2. What is a recursion tree? A recursion tree is a diagram that represents recursive function calls as a tree structure. It helps visualize how many calls occur and how the problem is divided.
Q3. What is the practical risk of exponential algorithms? Exponential algorithms grow extremely fast and become impractical for large inputs due to excessive time and resource consumption.
---- EXPERIMENT 6 — Recursive Binary Search ---- Q1. Why must data be sorted for binary search? Binary search works by comparing the target with the middle element and deciding which half to search. This is only possible if the data is sorted.
Q2. What are best, average, and worst case complexities of binary search? Best case: O(1) when target is middle element. Average case: O(log n) due to repeated halving. Worst case: O(log n) when search continues until one element remains.
Q3. What is divide and conquer? Divide and conquer is an algorithm design technique where a problem is divided into smaller subproblems, solved individually, and combined to form the final solution. Binary search is an example of divide and conquer.
