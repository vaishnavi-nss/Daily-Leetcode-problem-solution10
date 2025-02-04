# Daily-Leetcode-problem-solution10
PROBLEM

Given an array of positive integers nums, return the maximum possible sum of an ascending subarray in nums.
A subarray is defined as a contiguous sequence of numbers in an array.
A subarray [numsl, numsl+1, ..., numsr-1, numsr] is ascending if for all i where l <= i < r, numsi  < numsi+1. Note that a subarray of size 1 is ascending.

Approach

Initialize maxSum to store the maximum ascending subarray sum and currentSum with the first element.
Iterate through nums:
If the current number is greater than the previous one, extend the subarray and add the value to currentSum.
Otherwise, update maxSum if currentSum is greater, then reset currentSum to the current number.
Return the maximum of maxSum and currentSum after the loop ends.

Complexity

Time complexity:
O(n)

Space complexity:
O(1)
