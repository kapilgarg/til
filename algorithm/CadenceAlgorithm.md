## Cadence Algorithm
largest sum of a contiguous array 
https://leetcode.com/problems/maximum-subarray/ 

Maintain a global and local max sum. 
Initialize local sum to 0. 
Iterate from left to right.
### If adding the current number to local sum

1. Increases the local sum more than current number, contiguous array includes elements for the previous sum and current element
2. Increases the local sum but local sum is less than current number, only current number is in contiguous array.
3. Decreases the local sum, only previous sum and elements are in contiguous array.
4. Whenever local sum is greater than global sum, update global sum with local sum


