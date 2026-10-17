# Week-4-STEP-ASSIGNMENT
A1. Product of Array Except Self

Algorithm:

Create an output array of the same length as the input array.
Initialize a prefix product to 1.
Traverse from left to right, store the prefix product at each index, and update it by multiplying the current element.
Initialize a suffix product to 1.
Traverse from right to left, multiply each output element by the suffix product, and update the suffix product.
Return the output array.

Time Complexity: O(n)
Space Complexity: O(1) auxiliary space, excluding the output array.

A2. Maximum Subarray

Algorithm: Kadane's Algorithm

Initialize the current sum and maximum sum with the first element.
Traverse the array from the second element to the last element.
At each element, choose the maximum between the current element and the current sum plus that element.
Update the maximum sum if the current sum is greater.
Return the maximum sum.

Time Complexity: O(n)
Space Complexity: O(1)

A3. 3Sum

Algorithm: Sorting and Two Pointers

Sort the input array in ascending order.
Fix one element using a loop from index 0 to n − 3.
Skip the element if it is a duplicate of the previous element.
Initialize two pointers: left = i + 1 and right = n − 1.
Calculate the sum of the three elements.
If the sum is zero, store the triplet and move both pointers inward.
If the sum is less than zero, move the left pointer forward.
If the sum is greater than zero, move the right pointer backward.
Skip duplicate values at both pointers to avoid repeated triplets.
Return all unique triplets.

Time Complexity: O(n²)
Space Complexity: O(1) auxiliary space, excluding output and sorting-related space.

A4. Subarray Sum Equals K

Algorithm: Prefix Sum and HashMap

Create a HashMap to store prefix sums and their frequencies.
Initialize the map with prefix sum 0 having frequency 1.
Initialize the running prefix sum and count to 0.
Traverse the array and add each element to the running prefix sum.
Calculate prefix sum − k.
Add the frequency of this value in the HashMap to the count.
Increase the frequency of the current prefix sum in the HashMap.
Return the total count.

Time Complexity: O(n) average
Space Complexity: O(n)

A5. Find Minimum in Rotated Sorted Array

Algorithm: Binary Search

Initialize left = 0 and right = n − 1.
Repeat while left is less than right.
Calculate the middle index.
If the middle element is greater than the rightmost element, set left = mid + 1.
Otherwise, set right = mid.
When left equals right, return the element at that index.

Time Complexity: O(log n)
Space Complexity: O(1)

Note: A5 assumes a rotated sorted array with distinct elements.
