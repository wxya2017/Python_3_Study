# 你可以留下你想问的问题，并且把它put上来
把列表中的0都移动到最后：
def moveZeroes(nums):
    len_origin = len(nums)
    for num in nums:
        if num == 0: 
            nums.remove(num)
    len0 = len_origin - len(nums）
    for i in range(len0):
        nums.append(0)
        return nums
moveZeroes([0,0,1])
应该输出[1,0,0]，但是输出[0,1,0]
