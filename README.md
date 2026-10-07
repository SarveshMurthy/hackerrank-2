# HackerRank Algorithmic Problem-Solving & Portfolio

**Name:** Sarvesh Murthy
**SRN:** R25EJ081
**Course:** B.Tech CSIT — 3rd Semester  
**Activity:** Activity 8 — HackerRank Algorithmic Problem-Solving & Portfolio Integration  
**Course Code:** B25CS0311  

---

## 📌 About This Repository

This repository contains my solutions for **Activity 8: HackerRank Algorithmic Problem-Solving & Portfolio Integration**.

The activity focuses on developing algorithmic problem-solving skills through **array manipulation, matrix traversal, string processing, hash maps, data structures, bitwise operations, and algorithmic efficiency**.

All five required problems were successfully solved and verified on HackerRank, with **all test cases passing**.

---

## 🔗 Profiles

- **HackerRank:** `[https://www.hackerrank.com/profile/09saru1]`
- **GitHub:** `[https://github.com/SarveshMurthy]`

---

## 🏆 HackerRank Achievement

As part of this activity, I successfully achieved the required **3-Star Badge on HackerRank**.

### HackerRank Profile & 3-Star Badge

![HackerRank Profile and 3-Star Badge](screenshots/profile.png)

---

# 🧩 Problems Solved

| # | Problem | Topic | Time Complexity | Space Complexity | Status |
|---|---|---|---|---|---|
| 1 | [Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem) | 2D Arrays / Matrices | O(N) | O(1) | ✅ Accepted |
| 2 | [Dynamic Array](https://www.hackerrank.com/challenges/dynamic-array/problem) | Data Structures / Vectors | O(Q) Amortized | O(Q) | ✅ Accepted |
| 3 | [Time Conversion](https://www.hackerrank.com/challenges/time-conversion/problem) | Strings / Logic | O(1) | O(1) | ✅ Accepted |
| 4 | [Compare the Triplets](https://www.hackerrank.com/challenges/compare-the-triplets/problem) | Basic Implementation | O(1) | O(1) | ✅ Accepted |
| 5 | [Sparse Arrays](https://www.hackerrank.com/challenges/sparse-arrays/problem) | Hash Maps / Strings | O(N + Q) | O(N) | ✅ Accepted |

---

# 📂 Repository Structure

```text
hackerrank-2/
│
├── README.md
├── diagonaldifference.c
├── dynamicarray.c
├── timeconversion.c
├── comparetriplets.c
├── sparcearray.c
├── screenshots/
│   ├── 01-result.png
│   ├── 02-result.png
│   ├── 03-result.png
│   ├── 04-result.png
│   ├── 05-result.png
│   └── profile.png
└── .git/
```

---

# 1. Diagonal Difference

### 🔗 HackerRank Problem

[Diagonal Difference](https://www.hackerrank.com/challenges/diagonal-difference/problem)

### Problem

Given a square matrix, calculate the absolute difference between the sums of its primary diagonal and secondary diagonal.

### Approach

The primary diagonal is accessed using:

```cpp
matrix[i][i]
```

The secondary diagonal is accessed using:

```cpp
matrix[i][n - 1 - i]
```

Both diagonal sums can be calculated in a single traversal of the matrix.

### Complexity

- **Time:** O(N)
- **Space:** O(1)

### Result

✅ All HackerRank test cases passed.

### Solution

The complete C solution is available in:

```text
diagonaldifference.c
```

---

# 2. Dynamic Array

### 🔗 HackerRank Problem

[Dynamic Array](https://www.hackerrank.com/challenges/dynamic-array/problem)

### Problem

Implement a dynamic array data structure using multiple sequences and process queries based on a bitwise XOR operation involving the current `lastAnswer`.

### Approach

A collection of dynamic sequences is maintained using C++ vectors.

For every query, the target sequence is determined using:

```cpp
idx = (x ^ lastAnswer) % N;
```

For a Type 1 query, the value is appended to the selected sequence.

For a Type 2 query, an element is retrieved from the selected sequence and used to update `lastAnswer`.

### Complexity

- **Time:** O(Q) amortized
- **Space:** O(Q)

where `Q` represents the number of queries and the maximum number of elements stored across the sequences.

### Result

✅ All HackerRank test cases passed.

### Solution

The complete C solution is available in:

```text
dynamicarray.c
```

---

# 3. Time Conversion

### 🔗 HackerRank Problem

[Time Conversion](https://www.hackerrank.com/challenges/time-conversion/problem)

### Problem

Convert a time from **12-hour AM/PM format** into **24-hour format**.

Example:

```text
07:05:45PM → 19:05:45
```

### Approach

The hour portion is modified depending on whether the time is AM or PM.

The following cases are handled:

- PM hours other than 12 are increased by 12.
- `12 PM` remains `12`.
- `12 AM` becomes `00`.
- Other AM values remain unchanged.

### Complexity

- **Time:** O(1)
- **Space:** O(1)

### Result

✅ All HackerRank test cases passed.

### Solution

The complete C solution is available in:

```text
timeconversion.c
```

---

# 4. Compare the Triplets

### 🔗 HackerRank Problem

[Compare the Triplets](https://www.hackerrank.com/challenges/compare-the-triplets/problem)

### Problem

Compare the corresponding ratings of Alice and Bob and calculate their respective scores.

### Approach

Each of the three corresponding elements is compared individually.

- If Alice's value is greater, Alice receives one point.
- If Bob's value is greater, Bob receives one point.
- If both values are equal, neither receives a point.

### Complexity

- **Time:** O(1)
- **Space:** O(1)

### Result

✅ All HackerRank test cases passed.

### Solution

The complete C solution is available in:

```text
comparetriplets.c
```

---

# 5. Sparse Arrays

### 🔗 HackerRank Problem

[Sparse Arrays](https://www.hackerrank.com/challenges/sparse-arrays/problem)

### Problem

Given a collection of strings and a list of queries, determine how many times each query string occurs in the original collection.

### Approach

A frequency map is used to store the number of occurrences of every string.

Each query can then be answered using a direct lookup instead of repeatedly scanning the entire collection.

This improves the overall efficiency of the solution.

### Complexity

- **Time:** O(N + Q)
- **Space:** O(N)

where `N` is the number of input strings and `Q` is the number of queries.

### Result

✅ All HackerRank test cases passed.

### Solution

The complete C solution is available in:

```text
sparcearray.c
```

---

# 📊 Complexity Analysis

| Problem | Time Complexity | Space Complexity |
|---|---:|---:|
| Diagonal Difference | O(N) | O(1) |
| Dynamic Array | O(Q) Amortized | O(Q) |
| Time Conversion | O(1) | O(1) |
| Compare the Triplets | O(1) | O(1) |
| Sparse Arrays | O(N + Q) | O(N) |

The solutions prioritize efficient approaches and avoid unnecessary nested loops or repeated searches wherever possible.

---

# 📸 HackerRank Verification

## HackerRank Profile & 3-Star Badge

![HackerRank Profile and 3-Star Badge](screenshots/profile.png)

---

# ✅ Accepted Submissions

## 1. Dynamic Array

![Dynamic Array Result](screenshots/01-result.png)

---

## 2. Compare the Triplets

![Compare the Triplets Result](screenshots/02-result.png)

---

## 3. Diagonal Difference

![Diagonal Difference Result](screenshots/03-result.png)

---

## 4. Sparse Arrays

![Sparse Arrays Result](screenshots/04-result.png)

---

## 5. Time Conversion

![Time Conversion Result](screenshots/05-result.png)

---

# 💡 Key Learning Outcomes

Through this activity, I strengthened my understanding of:

- Array and matrix traversal
- Dynamic data structures and vectors
- String manipulation
- Hash maps and frequency counting
- Bitwise XOR operations
- Algorithmic time and space complexity
- Efficient data processing
- Optimizing solutions to avoid unnecessary repeated operations
- Writing clean and structured C solutions
- Testing and verifying solutions through HackerRank
- Maintaining a structured programming portfolio using GitHub

---

# 📝 Reflection

This activity helped me improve my algorithmic problem-solving skills by requiring me to focus not only on producing the correct output but also on developing efficient solutions.

Working with problems such as **Diagonal Difference** and **Sparse Arrays** demonstrated how carefully designed traversal techniques and frequency maps can reduce unnecessary operations. The **Dynamic Array** problem improved my understanding of vectors, nested sequences, and bitwise XOR operations. **Time Conversion** and **Compare the Triplets** strengthened my ability to implement straightforward logic clearly and efficiently.

A major learning outcome was understanding the importance of **time and space complexity**. Instead of relying on brute-force approaches, I learned to identify situations where more efficient solutions are preferable, particularly when processing larger inputs. The use of hash maps for frequency-based problems is one example of how additional memory can improve execution time.

Completing the problems on HackerRank and achieving the required **3-Star Badge** provided practical experience with an industry-recognized coding platform. Organizing the solutions, verification screenshots, and documentation in GitHub also helped me understand how to maintain a structured technical portfolio.

Overall, this activity improved my **algorithmic thinking, coding efficiency, debugging ability, and technical documentation skills**. It also gave me greater confidence in solving programming problems using C++ and presenting my work professionally.

---

# 🎯 Activity Completion

| Requirement | Status |
|---|---|
| Diagonal Difference | ✅ Completed |
| Dynamic Array | ✅ Completed |
| Time Conversion | ✅ Completed |
| Compare the Triplets | ✅ Completed |
| Sparse Arrays | ✅ Completed |
| All HackerRank Tests Passed | ✅ Completed |
| 3-Star HackerRank Badge | ✅ Achieved |
| GitHub Repository | ✅ Completed |
| Screenshots | ✅ Added |
| Reflection | ✅ Completed |

---

# 🏁 Final Status

**Activity 8 — HackerRank Algorithmic Problem-Solving & Portfolio Integration**

### **STATUS: COMPLETED ✅**

All five required HackerRank problems were successfully solved, tested, and documented. The required **3-Star HackerRank Badge** was also achieved, and the solutions have been organized into a structured GitHub portfolio.

---

**Sarvesh Murthy**  
**B.Tech CSIT — 3rd Semester**  
**Activity 8 — HackerRank Algorithmic Problem-Solving & Portfolio Integration**