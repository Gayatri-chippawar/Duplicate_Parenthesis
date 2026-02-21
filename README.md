# 🧠 Duplicate Parenthesis Detection (Java)
## 📌 Overview

This project implements an algorithm to detect duplicate (redundant) parentheses in a mathematical expression using the Stack data structure in Java.

Duplicate parentheses are unnecessary brackets that do not affect the expression’s evaluation.

## ✅ Example
Expression	Output
(a+b)	No duplicate
((a+b))	Duplicate present
(a+(b)/c)	Duplicate present
(a+b*(c-d))	No duplicate
## 🚀 Problem Statement

Given a balanced expression containing parentheses, determine whether the expression contains duplicate parentheses.

Duplicate parentheses exist if there is no operator or operand between a pair of parentheses.

Example:

((a+b))

The outer parentheses wrap an already valid (a+b) without adding any operation → Duplicate.

## 🛠️ Approach Used
🔹 Data Structure:

Stack<Character>

🔹 Algorithm Logic:

Traverse the expression character by character.

Push characters into the stack until ) is found.

When ) is encountered:

Check the top of the stack.

If the top is ( → duplicate parentheses found.

Otherwise:

Pop elements until ( is found.

Remove the matching (.

Continue until the expression ends.

## ⏱️ Time & Space Complexity
Complexity Type	Value
Time Complexity	O(n)
Space Complexity	O(n)

Each character is pushed and popped at most once.

Stack may store up to n characters in worst case.

## 🎯 Key Concepts Practiced

Stack implementation

Expression parsing

Parenthesis matching

Problem-solving using data structures

Time complexity analysis

## 📚 Learning Outcome

Through this implementation, you practiced:

Using stacks for expression-based problems

Detecting redundant structures

Writing clean and optimized Java logic

Handling edge cases in balanced expressions

## 🔎 Edge Cases Handled

Nested parentheses

No parentheses

Multiple duplicates

Balanced expressions

## 🏁 Conclusion

This project strengthens understanding of:

Stack-based algorithms

Expression validation problems (common in interviews)

Efficient traversal techniques

It is a frequently asked DSA interview problem, especially in stack and expression evaluation topics.
