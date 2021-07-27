# If a sorted array has duplicate elements  
a = [1,2,3,4,4,4,5,6]

## find left most element
1. l =0, r= len(n) 
2. run a loop till l < r => m=(l+2)//2
3. if a[m] is less than target, move right = > l = m+1
4. else move left => r = m
5. return l


## find right most elemnent 
all the steps are same as previous except #3 and #4
if a[m] > target, move left => r = m 
else move right => l = m+1

## Rank query 
find left most element can also be used used to find the rank of an element. Rank is the number of elements before the target element. return value is the number of elements before target value.



