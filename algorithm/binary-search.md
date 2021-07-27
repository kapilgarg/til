# If a sorted array has duplicate elements  
a = [1,2,3,4,4,4,5,6]

## Find left most element
1. l =0, r= len(n) 
2. run a loop till l < r => m=(l+2)//2
3. if a[m] is less than target, move right = > l = m+1
4. else move left => r = m
5. return l 

```python
def bs_l(nums,t):
    nums.sort()
    l,r = 0,len(nums)
    while l<r:
        m = (l+r)//2
        if nums[m]<t:
            l=m+1
        else:
            r=m
    return l,nums[l]
```

## Find right most elemnent 
all the steps are same as previous except #3 and #4
if a[m] > target, move left => r = m 
else move right => l = m+1 

```python
def bs_r(nums,t):
    nums.sort()
    l,r = 0,len(nums)
    while l<r:
        m = (l+r)//2
        if nums[m]>t:
            r = m
        else:
            l=m+1
    return r-1
```

## Rank query 
**Find left most element** can also be used used to find the _rank of an element_. Rank is the number of elements before the target element. return value is the number of elements before target value. Using the rank, we can also find the predecessor (rank-1) or successor (rank or rank+1)

From the bs_l function, rank of 5 in array [1,2,3,4,7,8,10,11,13,14,15] 

 = **4** which means there are 4 elements before this. If the target is present, its index would be 4 .





