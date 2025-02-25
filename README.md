QUESTION 1:- Merge Sorted Array:-You are given two integer arrays nums1 and nums2, sorted in non-decreasing order, and two integers m and n, representing the number of elements in nums1 and nums2 respectively.Merge nums1 and nums2 into a single array sorted in non-decreasing order.The final sorted array should not be returned by the function, but instead be stored inside the array nums1. To accommodate this, nums1 has a length of m + n, where the first m elements denote the elements that should be merged, and the last n elements are set to 0 and should be ignored. nums2 has a length of n.

Example 1:Input: nums1 = [1,2,3,0,0,0], m = 3, nums2 = [2,5,6], n = 3Output: [1,2,2,3,5,6]Explanation: The arrays we are merging are [1,2,3] and [2,5,6].The result of the merge is [1,2,2,3,5,6] with the underlined elements coming from nums1.

Example 2:Input: nums1 = [1], m = 1, nums2 = [], n = 0Output: [1]Explanation: The arrays we are merging are [1] and [].The result of the merge is [1].Example 3:Input: nums1 = [0], m = 0, nums2 = [1], n = 1Output: [1]Explanation: The arrays we are merging are [] and [1].The result of the merge is [1].Note that because m = 0, there are no elements in nums1. The 0 is only there to ensure the merge result can fit in nums1. 

Constraints:nums1.length == m + nnums2.length == n0 <= m, n <= 2001 <= m + n <= 200-109 <= nums1[i], nums2[j] <= 109


QUESTION 2:- FIRST BAD VERSION:-You are a product manager and currently leading a team to develop a new product. Unfortunately, the latest version of your product fails the quality check. Since each version is developed based on the previous version, all the versions after a bad version are also bad.Suppose you have n versions [1, 2, ..., n] and you want to find out the first bad one, which causes all the following ones to be bad.You are given an API bool isBadVersion(version) which returns whether version is bad. Implement a function to find the first bad version. You should minimize the number of calls to the API.

Example 1:Input: n = 5, bad = 4Output: 4Explanation:call isBadVersion(3) -> falsecall isBadVersion(5) -> truecall isBadVersion(4) -> trueThen 4 is the first badversion.
Example 2:Input: n = 1, bad = 1Output: 1
Constraints:1 <= bad <= n <= 231 - 1


QUESTION3:- SORT COLORS:- Given an array nums with n objects colored red, white, or blue, sort them in-place so that objects of the same color are adjacent, with the colors in the order red, white, and blue.We will use the integers 0, 1, and 2 to represent the color red, white, and blue, respectively.
You must solve this problem without using the library's sort function.

Example 1:Input: nums = [2,0,2,1,1,0] Output: [0,0,1,1,2,2]

Example 2: Input: nums = [2,0,1]
Output: [0,1,2]
Constraints:n == nums.length 1 <= n <= 300 nums[i] is either 0, 1, or 2.


QUESTION 4:- MEDIAN OF TWO SORTED ARRAYS:-Given two sorted arrays nums1 and nums2 of size m and n respectively, return the median of the two sorted arrays.The overall run time complexity should be O(log (m+n)). 
Example 1:
Input: nums1 = [1,3], nums2 = [2]
Output: 2.00000
Explanation: merged array = [1,2,3] and median is 2.

Example 2:
Input: nums1 = [1,2], nums2 = [3,4]
Output: 2.50000
Explanation: merged array = [1,2,3,4] and median is (2 + 3) / 2 = 2.5.

Constraints:
nums1.length == m
nums2.length == n
0 <= m <= 1000
0 <= n <= 1000
1 <= m + n <= 2000
-106 <= nums1[i], nums2[i] <= 106


QUESTION 5:-KTH SMALLEST ELEMENT IN A SORTED MATRIX:-Given an n x n matrix where each of the rows and columns is sorted in ascending order, return the kth smallest element in the matrix.Note that it is the kth smallest element in the sorted order, not the kth distinct element.You must find a solution with a memory complexity better than O(n2).
Example 1:
Input: matrix = [[1,5,9],[10,11,13],[12,13,15]], k = 8
Output: 13
Explanation: The elements in the matrix are [1,5,9,10,11,12,13,13,15], and the 8th smallest number is 13

Example 2:
Input: matrix = [[-5]], k = 1
Output: -5
 
Constraints:
n == matrix.length == matrix[i].length
1 <= n <= 300
-109 <= matrix[i][j] <= 109
All the rows and columns of matrix are guaranteed to be sorted in non-decreasing order.
1 <= k <= n2
