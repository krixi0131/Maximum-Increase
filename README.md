# Maximum-Increase
You are given array consisting of n integers. Your task is to find the maximum length of an increasing subarray of the given array.

A subarray is the sequence of consecutive elements of the array. Subarray is called increasing if each element of this subarray strictly greater than previous.

Input
The first line contains single positive integer n (1 ≤ n ≤ 105) — the number of integers.

The second line contains n positive integers a1, a2, ..., an (1 ≤ ai ≤ 109).

Output
Print the maximum length of an increasing subarray of the given array.
```python
n=int(input())
a=list(map(int,input().split()))
ans=1
ma=1
for i in range(n-1):
    if a[i+1]>a[i]:
        ans+=1
    else:
        ans=1
    ma=max(ans,ma)
print(ma)
```
