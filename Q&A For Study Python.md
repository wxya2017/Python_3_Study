# 你可以留下你想问的问题，并且把它put上来
Given an array nums, write a function to move all 0's to the end of it while maintaining the relative order of the non-zero elements.

For example, given nums = [0, 1, 0, 3, 12], after calling your function, nums should be [1, 3, 12, 0, 0].

Note:
You must do this in-place without making a copy of the array.
Minimize the total number of operations.


    def moveZeroes(nums):
        """
        :type nums: List[int]
        :rtype: void Do not return anything, modify nums in-place instead.
        """

        len_origin = len(nums)
        for num in nums:
            if num == 0: 
                nums.remove(num)
        len0 = len_origin - len(nums)
        for i in range(0,len0):
            nums.append(0)
        return nums
    moveZeroes([0,0,1])

# [0,0,1]? output [0,1,0] 应该是 [0,0,1]
