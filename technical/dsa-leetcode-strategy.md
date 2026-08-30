---
title: "DSA & LeetCode strategy"
author:
  name: "progsu team"
  handle: "@progsu"
readTime: "12 min read"
publishDate: 2026-02-24T00:00:00.000Z
updated: 2026-05-28T00:00:00.000Z
tags: [dsa, leetcode, technical-interview, algorithms]
category: technical
---

# DSA & LeetCode strategy


## why DSA matters

every major tech company tests data structures and algorithms in their interviews. whether it's FAANG, startups, or mid-size companies, you **will** be asked to solve coding problems on a whiteboard or in a shared editor.

- the good news: there are only ~15 core patterns that cover 90%+ of interview questions
- the bad news: you can't cram this in a weekend; it takes consistent practice
- the strategy below gives you a structured path from zero to interview-ready

> [!tip]
> **quick Tip:** Don't grind 500 random problems. focus on **patterns** first, then apply them across problems. quality over quantity.

---

# the strategy: how to actually study

## step 1: learn the pattern, not just the problem

every problem below belongs to a **pattern category**. before solving problems, understand the pattern:

1. **watch the video solution** first to understand the approach
2. **code it yourself** without looking; struggle is where learning happens
3. **if stuck for 20+ minutes**, re-watch the video and try again
4. **review your solution**: can you explain it out loud?

## step 2: follow the roadmap in order

the problems below are organized from **Foundation to Expert**. each level builds on the previous one. don't skip ahead; the patterns compound.

## step 3: track your progress

track which problems you've completed and compete with others using the practice link above.

> [!warning]
> **important:** Aim for **2-3 problems per day** consistently rather than 20 problems in one day. spaced repetition is how you retain patterns.

---

# foundation level

these are your building blocks. master these before moving on; nearly every harder problem uses these patterns.

## arrays + hashing

> foundation for most problems: efficient lookups and storage.

**core idea:** Use hash maps for O(1) lookups instead of brute-force nested loops. if you're writing two nested for-loops, there's almost always a hash map solution.

**strategy:**
- always ask: "Can I trade space for time with a hash map?"
- for frequency problems, use a counter/dictionary
- for "find pair" problems, store complements in a set

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Two Sum | [Video](https://www.youtube.com/watch?v=KLlXCFG5TnA) |
| 2 | Contains Duplicate | [Video](https://www.youtube.com/watch?v=3OamzN90kPg) |
| 3 | Group Anagrams | [Video](https://www.youtube.com/watch?v=vzdNOK2oB2E) |
| 4 | Top K Frequent Elements | [Video](https://www.youtube.com/watch?v=YPTqKIgVk-k) |
| 5 | Product of Array Except Self | [Video](https://www.youtube.com/watch?v=yKZFurr4GQA) |
| 6 | Encode and Decode Strings | [Video](https://www.youtube.com/watch?v=B1k_sxOSgv8) |
| 7 | Longest Consecutive Sequence | [Video](https://www.youtube.com/watch?v=P6RZZMu_maU) |
| 8 | Maximum Subarray Sum | [Video](https://www.youtube.com/watch?v=5WZl3MMT0Eg) |

---

## two pointers

> builds on arrays to solve search and pairing problems.

**core idea:** Use two pointers moving toward each other (or in the same direction) to reduce O(n^2) to O(n). works best on **sorted arrays**.

**strategy:**
- sort the array first if not already sorted
- left pointer starts at beginning, right at end
- move the pointer that gets you closer to your target

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Valid Palindrome | [Video](https://www.youtube.com/watch?v=jJXJ16kPFWg) |
| 2 | Two Sum II - Input Array Is Sorted | [Video](https://www.youtube.com/watch?v=cQ1Oz4ckceM) |
| 3 | Container With Most Water | [Video](https://www.youtube.com/watch?v=UuiTKBwPgAo) |
| 4 | 3Sum | [Video](https://www.youtube.com/watch?v=jzZsG8n2R9A) |
| 5 | Move Zeroes | [Video](https://www.youtube.com/watch?v=aayNRwUN3Do) |
| 6 | Remove Duplicates from Sorted Array | [Video](https://www.youtube.com/watch?v=DEJAZBq0FDA) |
| 7 | Trapping Rain Water | [Video](https://www.youtube.com/watch?v=ZI2z5pq0TqA) |

---

## stack

> adds memory of previous elements: great for parsing and monotonic problems.

**core idea:** Use a stack when you need to remember previous elements and process them in reverse order (LIFO). if you see nested structures or "next greater/smaller" patterns, think stack.

**strategy:**
- matching brackets/parentheses = stack
- "next greater element" = monotonic stack
- evaluate expressions = stack with operators

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Valid Parentheses | [Video](https://www.youtube.com/watch?v=WTzjTskDFMg) |
| 2 | Min Stack | [Video](https://www.youtube.com/watch?v=qkLl7nAwDPo) |
| 3 | Evaluate Reverse Polish Notation | [Video](https://www.youtube.com/watch?v=iu0082c4HDE) |
| 4 | Daily Temperatures | [Video](https://www.youtube.com/watch?v=cTBiBSnjO3c) |
| 5 | Car Fleet | [Video](https://www.youtube.com/watch?v=Pr6T-3yB9RM) |
| 6 | Largest Rectangle in Histogram | [Video](https://www.youtube.com/watch?v=zx5Sw9130L0) |

---

## binary search

> builds on arrays for sorted search optimization.

**core idea:** If the input is sorted (or has a monotonic property), you can eliminate half the search space each step. O(log n) instead of O(n).

**strategy:**
- classic binary search: find target in sorted array
- "minimum/maximum that satisfies condition" = binary search on answer
- always check: can I binary search the search space?

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Search a 2D Matrix | [Video](https://www.youtube.com/watch?v=Ber2pi2C0j0) |
| 2 | Search in Rotated Sorted Array | [Video](https://www.youtube.com/watch?v=U8XENwh8Oy8) |
| 3 | Find Minimum in Rotated Sorted Array | [Video](https://www.youtube.com/watch?v=nIVW4P8b1VA) |
| 4 | Koko Eating Bananas | [Video](https://www.youtube.com/watch?v=U2SozAs9RzA) |
| 5 | Median of Two Sorted Arrays | [Video](https://www.youtube.com/watch?v=q6IEA26hvXc) |

---

## sliding window

> extends array logic for subarray optimization.

**core idea:** Maintain a "window" over a contiguous subarray/substring. expand the right side, shrink the left side when constraints are violated. turns O(n^2) substring problems into O(n).

**strategy:**
- "longest/shortest substring with condition" = sliding window
- use a hash map to track window contents
- expand right pointer, shrink left when window is invalid

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Longest Substring Without Repeating Characters | [Video](https://www.youtube.com/watch?v=wiGpQwVHdE0) |
| 2 | Minimum Window Substring | [Video](https://www.youtube.com/watch?v=jSto0O4AJbM) |
| 3 | Permutation in String | [Video](https://www.youtube.com/watch?v=UbyhOgBN834) |
| 4 | Longest Repeating Character Replacement | [Video](https://www.youtube.com/watch?v=gqXU1UyA8pk) |
| 5 | Sliding Window Maximum | [Video](https://www.youtube.com/watch?v=DfljaUwZsOk) |

---

# intermediate level

linked & hierarchical structures. these build on your foundation patterns and introduce pointer manipulation and recursion.

## linked list

**core idea:** Pointer manipulation. most linked list problems are about rewiring `.next` pointers. draw it out on paper first.

**strategy:**
- use a **dummy node** to simplify edge cases (empty list, single node)
- **fast and slow pointers** detect cycles and find midpoints
- reverse a linked list is a building block for many harder problems

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Reverse Linked List | [Video](https://www.youtube.com/watch?v=G0_I-ZF0S38) |
| 2 | Linked List Cycle | [Video](https://www.youtube.com/watch?v=gBTe7lFR3vc) |
| 3 | Remove Nth Node From End | [Video](https://www.youtube.com/watch?v=XVuQxVej6y8) |
| 4 | Reorder List | [Video](https://www.youtube.com/watch?v=Pno7rUOZM-o) |
| 5 | Add Two Numbers | [Video](https://www.youtube.com/watch?v=wgFPrzTjm7s) |

---

## trees

**core idea:** Most tree problems are solved with **DFS** (recursive) or **BFS** (level-order with a queue). the recursive structure of trees maps naturally to recursive solutions.

**strategy:**
- ask: "Can I solve this with a recursive DFS?" - usually yes
- for level-by-level processing, use BFS with a queue
- BST property: left < root < right; use this for validation and search

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Invert Binary Tree | [Video](https://www.youtube.com/watch?v=OnSn2XEQ4MY) |
| 2 | Same Tree | [Video](https://www.youtube.com/watch?v=vRbbcKXCxOw) |
| 3 | Subtree of Another Tree | [Video](https://www.youtube.com/watch?v=E36O5SWp-LE) |
| 4 | Lowest Common Ancestor | [Video](https://www.youtube.com/watch?v=13m9ZCB8gjw) |
| 5 | Binary Tree Level Order Traversal | [Video](https://www.youtube.com/watch?v=Ke90Tje7VS0) |
| 6 | Validate Binary Search Tree | [Video](https://www.youtube.com/watch?v=s6ATEkipzow) |
| 7 | Kth Smallest Element in a BST | [Video](https://www.youtube.com/watch?v=5LUXSvjmGCw) |

---

## tries

**core idea:** A trie (prefix tree) stores strings character by character. perfect for prefix matching, autocomplete, and word search problems.

**strategy:**
- if the problem involves prefixes or dictionary lookups, think trie
- each node has up to 26 children (for lowercase English)
- mark end-of-word nodes to distinguish complete words from prefixes

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Implement Trie (Prefix Tree) | [Video](https://www.youtube.com/watch?v=AXjmTQ8LEoI) |
| 2 | Design Add and Search Words Data Structure | [Video](https://www.youtube.com/watch?v=BTf05gs_8iU) |
| 3 | Replace Words | [Video](https://www.youtube.com/watch?v=EHjHJnkQ_XQ) |
| 4 | Word Search II | [Video](https://www.youtube.com/watch?v=U6OGOZ2N5-w) |

---

# advanced patterns

recursion & optimization. these patterns are harder but show up frequently in interviews at top companies.

## backtracking

**core idea:** Build solutions incrementally and abandon ("backtrack") paths that can't lead to a valid solution. it's DFS on a decision tree.

**strategy:**
- draw the decision tree first
- at each step: make a choice, recurse, undo the choice
- prune early: skip branches that violate constraints

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Subsets | [Video](https://www.youtube.com/watch?v=REOH22Xwdkk) |
| 2 | Combination Sum | [Video](https://www.youtube.com/watch?v=GBKI9VSKdGg) |
| 3 | Permutations | [Video](https://www.youtube.com/watch?v=s7AvT7cGdSo) |
| 4 | N-Queens | [Video](https://www.youtube.com/watch?v=Ph95IHmRp5M) |
| 5 | Sudoku Solver | [Video](https://www.youtube.com/watch?v=nC1rbW2YSz0) |

---

## heap / priority queue

**core idea:** Efficiently track the min/max element. use a heap when you need repeated access to the smallest or largest item.

**strategy:**
- "top K" anything = heap
- use a **min heap** of size K to find the Kth largest
- use a **max heap** when you need the largest element quickly

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Kth Largest Element in a Stream | [Video](https://www.youtube.com/watch?v=hOjcdrqMoQ8) |
| 2 | Last Stone Weight | [Video](https://www.youtube.com/watch?v=iygakK8nK9Y) |
| 3 | Task Scheduler | [Video](https://www.youtube.com/watch?v=YCD_iYxyXoo) |
| 4 | Top K Frequent Words | [Video](https://www.youtube.com/watch?v=LEMkPoXLFcg) |
| 5 | Merge K Sorted Lists | [Video](https://www.youtube.com/watch?v=q5a5OiGbT6Q) |

---

## graphs

**core idea:** Model problems as nodes and edges. most graph problems use BFS (shortest path) or DFS (exploration/connected components).

**strategy:**
- "number of islands" type = DFS/BFS flood fill
- "shortest path" = BFS (unweighted) or Dijkstra (weighted)
- "can I complete all tasks?" = topological sort (cycle detection)
- always track visited nodes to avoid infinite loops

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Number of Islands | [Video](https://www.youtube.com/watch?v=pV2kpPD66nE) |
| 2 | Course Schedule | [Video](https://www.youtube.com/watch?v=EgI5nU9etnU) |
| 3 | Pacific Atlantic Water Flow | [Video](https://www.youtube.com/watch?v=s-VkcjHqkGI) |
| 4 | Rotten Oranges | [Video](https://www.youtube.com/watch?v=y704fEOx0s0) |
| 5 | Word Ladder | [Video](https://www.youtube.com/watch?v=h9iTnkgv05E) |

---

## dynamic programming (1-D)

**core idea:** Break a problem into overlapping subproblems. store results to avoid recomputation. if a recursive solution has repeated calls, DP can optimize it.

**strategy:**
- start with a **recursive** brute-force solution
- add **memoization** (top-down) or build a **DP table** (bottom-up)
- define your state clearly: `dp[i]` = what does index i represent?
- find the **recurrence relation**: how does `dp[i]` relate to previous values?

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Climbing Stairs | [Video](https://www.youtube.com/watch?v=Y0lT9Fck7qI) |
| 2 | Coin Change | [Video](https://www.youtube.com/watch?v=H9bfqozjoqs) |
| 3 | Word Break | [Video](https://www.youtube.com/watch?v=Sx9NNgInc3A) |
| 4 | Partition Equal Subset Sum | [Video](https://www.youtube.com/watch?v=IsvocB5BJhw) |

---

## dynamic programming (2-D)

**core idea:** Same as 1-D DP but with two changing variables. `dp[i][j]` usually represents a subproblem on a substring, subarray, or grid.

**strategy:**
- string comparison problems (edit distance, LCS) = 2D DP
- grid traversal problems (unique paths) = 2D DP
- draw out the DP table to visualize transitions

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Unique Paths | [Video](https://www.youtube.com/watch?v=IlEsdxuD4lY) |
| 2 | Longest Common Subsequence | [Video](https://www.youtube.com/watch?v=Ua0GhsJSlWM) |
| 3 | Distinct Subsequences | [Video](https://www.youtube.com/watch?v=-RDzMJ33nx8) |
| 4 | Edit Distance | [Video](https://www.youtube.com/watch?v=XYi2-LPrwm4) |

---

# expert level

optimization & logic. these are the patterns that separate good from great in interviews.

## intervals

**core idea:** Sort by start (or end) time, then process intervals linearly. most interval problems become simple after sorting.

**strategy:**
- sort intervals by start time
- compare current interval's start with previous interval's end
- merge, insert, or count based on overlap

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Meeting Rooms | [Video](https://www.youtube.com/watch?v=PaJxqZVPhbg) |
| 2 | Insert Interval | [Video](https://www.youtube.com/watch?v=A8NUOmlwOlM) |
| 3 | Non-overlapping Intervals | [Video](https://www.youtube.com/watch?v=nONCGxWoUfM) |
| 4 | Minimum Number of Arrows to Burst Balloons | [Video](https://www.youtube.com/watch?v=Z9oS6pC0QNM) |

---

## greedy

**core idea:** Make the locally optimal choice at each step. greedy works when the local optimum leads to the global optimum.

**strategy:**
- ask: "Does choosing the best option right now hurt future choices?"
- if not, greedy works
- often paired with sorting

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Maximum Subarray | [Video](https://www.youtube.com/watch?v=86CQq3pKSUw) |
| 2 | Valid Parenthesis String | [Video](https://www.youtube.com/watch?v=QhPdNS143Qg) |
| 3 | Gas Station | [Video](https://www.youtube.com/watch?v=lJwbPZGo05A) |
| 4 | Hand of Straights | [Video](https://www.youtube.com/watch?v=amnrMCVd2YI) |

---

## advanced graphs

**core idea:** Weighted graph algorithms. Dijkstra for shortest path, Prim's/Kruskal's for minimum spanning trees.

**strategy:**
- "shortest path with weights" = Dijkstra (use a min heap)
- "connect all nodes with minimum cost" = MST (Prim's or Kruskal's)

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Network Delay Time | [Video](https://www.youtube.com/watch?v=EaphyqKU4PQ) |
| 2 | Min Cost to Connect All Points | [Video](https://www.youtube.com/watch?v=f7JOBJIC-NA) |

---

## bit manipulation

**core idea:** Use binary operations (AND, OR, XOR, shifts) for O(1) space tricks. XOR is especially powerful: `a ^ a = 0` and `a ^ 0 = a`.

**strategy:**
- "find the single/missing number" = XOR everything
- count bits with `n & (n - 1)` to clear lowest set bit
- use bit shifts for powers of 2

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Single Number | [Video](https://www.youtube.com/watch?v=qMPX1AOa83k) |
| 2 | Number of 1 Bits | [Video](https://www.youtube.com/watch?v=5Km3utixwZs) |
| 3 | Counting Bits | [Video](https://www.youtube.com/watch?v=RyBM56RIWrM) |
| 4 | Missing Number | [Video](https://www.youtube.com/watch?v=WnPLSRLSANE) |
| 5 | Reverse Integer | [Video](https://www.youtube.com/watch?v=HAgLH58IgJQ) |

---

## math + geometry

**core idea:** Matrix manipulation, number theory, and spatial reasoning. these problems test your ability to think mathematically.

**strategy:**
- matrix rotation: transpose + reverse rows
- spiral traversal: track boundaries (top, bottom, left, right)
- for number problems, think about mathematical properties first

| # | Problem | Video Solution |
|---|---------|----------------|
| 1 | Rotate Image | [Video](https://www.youtube.com/watch?v=fMSJSS7eO1w) |
| 2 | Set Matrix Zeroes | [Video](https://www.youtube.com/watch?v=T41rL0L3Pnw) |
| 3 | Spiral Matrix | [Video](https://www.youtube.com/watch?v=BJnMZNwUk1M) |
| 4 | Valid Sudoku | [Video](https://www.youtube.com/watch?v=TjFXEUCMqI8) |
| 5 | Happy Number | [Video](https://www.youtube.com/watch?v=LWr4htY8d74) |
| 6 | Pow(x, n) | [Video](https://www.youtube.com/watch?v=g9YQyYi4IQQ) |

---

# interview day tips

> [!tip]
> **success Strategy:** During the actual interview, follow this framework for every problem:

1. **clarify** (1-2 min): Repeat the problem, ask about edge cases, confirm input/output
2. **plan** (3-5 min): Identify the pattern, explain your approach, discuss time/space complexity
3. **code** (15-20 min): Write clean code, talk through your logic as you go
4. **test** (3-5 min): Walk through an example, check edge cases, fix bugs

> [!warning]
> **important:** If you get stuck, **communicate**. say "I'm thinking about using X pattern because..."; interviewers want to see your thought process, not just the answer.

### common mistakes in interviews

- jumping straight into code without a plan
- going silent when stuck
- not testing your solution with examples
- ignoring edge cases (empty input, single element, duplicates)
- over-engineering when a simple solution works

### time complexity cheat sheet

| Complexity | Name | Example |
|-----------|------|---------|
| O(1) | Constant | Hash map lookup |
| O(log n) | Logarithmic | Binary search |
| O(n) | Linear | Single pass through array |
| O(n log n) | Linearithmic | Sorting |
| O(n^2) | Quadratic | Nested loops (usually avoidable) |
| O(2^n) | Exponential | Brute-force subsets |

---

see also: [[interview-guide]]
