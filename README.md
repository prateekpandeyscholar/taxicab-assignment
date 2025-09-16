# Assignment: Taxicab Numbers

## 📘 Problem Statement
A **Taxicab number** is the smallest number that can be expressed as the sum of two positive cubes in **two distinct ways**.  
For example, the first such number is:

```
1729 = 1³ + 12³ = 9³ + 10³
```

In this assignment, you will write a program to **find Taxicab numbers** up to a given limit `N`.

---

## ✅ Task
- Write a Java program that:
  1. Accepts an integer input `N`.
  2. Finds and prints all integers ≤ `N` that can be expressed as the sum of two cubes in at least two different ways.
  3. For each such number, print all distinct pairs `(a, b)` such that:
     ```
     a³ + b³ = number
     ```
  4. You may ignore `(a, b)` where `a > b` to avoid duplicates.

---

## 🔍 Example Output
For `N = 20000`, your program should output something like:

```
1729 = (1,12) (9,10)
4104 = (2,16) (9,15)
13832 = (2,24) (18,20)
...
```

---

## ⚙️ Instructions
1. Clone this repository into your local machine.
2. Complete the code in `src/Main.java`.
3. Commit and push your changes back to **your GitHub Classroom repository**.
4. No test cases are provided — submission is enough for completion.

---

## 💡 Hints
- Use a `HashMap<Integer, List<String>>` to store sums of cubes.
- Avoid double-counting pairs like `(a,b)` and `(b,a)` by starting inner loop from `b = a`.
- Check only sums that occur with **at least 2 different pairs**.

---

## 📤 Submission
- Push your solution code to your GitHub Classroom repository.
- Ensure that `src/Main.java` compiles and runs.

Good luck 🚀
