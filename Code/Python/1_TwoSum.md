# LeetCode Problem #1 — Two Sum

## Problem Description
Given an array of integers `nums` and an integer `target`, return **indices of the two numbers** such that they add up to `target`.  
You may assume that each input would have **exactly one solution**, and you may not use the same element twice.

---

## Solution (Python)

```python
class Solution(object):
    def twoSum(self, nums, target):
        """
        :type nums: List[int]
        :type target: int
        :rtype: List[int]
        """
        for i in range(0, len(nums)):
            for j in range(0, len(nums)):
                if i != j and nums[i] + nums[j] == target:
                    return [i, j]
                    break
```
## Example

Input: [2, 7, 11, 15]

Target: 9

Output: [0, 1]
