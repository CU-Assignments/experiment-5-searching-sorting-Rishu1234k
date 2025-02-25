QUESTION 1:- Merge Sorted Array:-You are given two integer arrays nums1 and nums2, sorted in non-decreasing order, and two integers m and n, representing the number of elements in nums1 and nums2 respectively.Merge nums1 and nums2 into a single array sorted in non-decreasing order.The final sorted array should not be returned by the function, but instead be stored inside the array nums1. To accommodate this, nums1 has a length of m + n, where the first m elements denote the elements that should be merged, and the last n elements are set to 0 and should be ignored. nums2 has a length of n.
Example 1:Input: nums1 = [1,2,3,0,0,0], m = 3, nums2 = [2,5,6], n = 3Output: [1,2,2,3,5,6]Explanation: The arrays we are merging are [1,2,3] and [2,5,6].The result of the merge is [1,2,2,3,5,6] with the underlined elements coming from nums1.
Example 2:Input: nums1 = [1], m = 1, nums2 = [], n = 0Output: [1]Explanation: The arrays we are merging are [1] and [].The result of the merge is [1].Example 3:Input: nums1 = [0], m = 0, nums2 = [1], n = 1Output: [1]Explanation: The arrays we are merging are [] and [1].The result of the merge is [1].Note that because m = 0, there are no elements in nums1. The 0 is only there to ensure the merge result can fit in nums1. 
Constraints:nums1.length == m + nnums2.length == n0 <= m, n <= 2001 <= m + n <= 200-109 <= nums1[i], nums2[j] <= 109


QUESTION 2:-You are a product manager and currently leading a team to develop a new product. Unfortunately, the latest version of your product fails the quality check. Since each version is developed based on the previous version, all the versions after a bad version are also bad.
Suppose you have n versions [1, 2, ..., n] and you want to find out the first bad one, which causes all the following ones to be bad.
You are given an API bool isBadVersion(version) which returns whether version is bad. Implement a function to find the first bad version. You should minimize the number of calls to the API.
Example 1:Input: n = 5, bad = 4Output: 4Explanation:call isBadVersion(3) -> falsecall isBadVersion(5) -> truecall isBadVersion(4) -> trueThen 4 is the first badversion.Example 2:Input: n = 1, bad = 1Output: 1
Constraints:1 <= bad <= n <= 231 - 1

QUESTION3:-
