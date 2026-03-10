# leetcode-problems
Problem 1: two sum 
Given an array of integers nums and an integer target, return indices of the two numbers such that they add up to target.

You may assume that each input would have exactly one solution, and you may not use the same element twice.

You can return the answer in any order.

Input: nums = [2,7,11,15], target = 9 solution for leetcode 
Output: [0,1]
Explanation: Because nums[0] + nums[1] == 9, we return [0, 1].


 Idea😍
For each number num in the array:

*Compute the complement needed to reach.
          ```
complement = target - num
```
*Check if the complement already exists in a hash map.

*If it exists → return the indices.

Otherwise store the current number with its index.

This gives O(n) time complexity instead of O(n²) brute force.


