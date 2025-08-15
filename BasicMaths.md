# Reverse Integer
https://leetcode.com/problems/reverse-integer/description/
```cpp
class Solution {
public:
    int reverse(int x) {
        if (x==INT_MIN) return 0;
        int d,rev=0,copy=abs(x);
        while (copy>0){
            d=copy%10;
            copy=copy/10;
            if (rev > INT_MAX/10 || rev< INT_MIN/10) return 0;
            rev=rev*10+d;
        }
        if (x<0) return -rev;
        return rev;
    }
};
```
