# Problem 1
https://cses.fi/problemset/task/1068
<img width="881" alt="Screenshot 2025-06-02 at 7 30 09 PM" src="https://github.com/user-attachments/assets/52f35a3b-dcea-4fb2-8c57-660601e14064" />  

### Here's my solution:  
```python
n=int(input())
while(True):
    print(n,end=" ")
    if(n==1) : break
    if n % 2 == 0:
        n = n // 2
    else:
        n = 3 * n + 1
```

