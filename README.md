# 977. Squares of a Sorted Array

## Problem
Given an integer array `nums` sorted in non-decreasing order, return an array containing the square of each number, also sorted in non-decreasing order.

**LeetCode:** [Squares of a Sorted Array](https://leetcode.com/problems/squares-of-a-sorted-array/)

**Difficulty:** Easy

## Approach: Two Pointers

1. Initialize `left` at the beginning and `right` at the end of the array.
2. Create a result array and initialize `pos` to its last index.
3. Compare the absolute values of the elements at `left` and `right`.
4. Square the element with the larger absolute value and store it at `result[pos]`.
5. Move the corresponding pointer inward and decrement `pos`.
6. Repeat until all elements have been processed.

Filling the result array from right to left ensures that the largest squares are placed first in the result's last positions.

## Complexity Analysis

- **Time Complexity:** `O(n)` — Each element is processed once.
- **Space Complexity:** `O(n)` — A separate result array is used.

## Key Concepts

- Two Pointers
- Arrays
- Absolute Value
- Time and Space Complexity
