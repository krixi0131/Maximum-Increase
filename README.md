# Maximum-Increase
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
