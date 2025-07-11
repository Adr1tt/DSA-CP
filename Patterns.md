# Star triangle
https://www.naukri.com/code360/problems/star-triangle_6573671?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems&leftPanelTabValue=PROBLEM
![image](https://github.com/user-attachments/assets/752faa64-5d28-456d-a9a3-e9e8d60d67f3)  
### My solution
```cpp
void nStarTriangle(int n) {
    for (int i=0;i<n;i++){
        for (int k=0; k<(n-i-1);k++){
            cout << " ";
        }
        for (int j=0;j<(2*i+1);j++){
            cout << "*";
        }
        cout << endl;
    }
}
```
---
# Reverse Star triangle
https://www.naukri.com/code360/problems/reverse-star-triangle_6573685?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems&leftPanelTabValue=SUBMISSION
![image](https://github.com/user-attachments/assets/a8215890-3cc0-4549-b606-8ddd166a73cf)
### My solution
```cpp
void nStarTriangle(int n) {
    for (int i=n-1;i>=0;i--){
        for (int k=0; k<(n-i-1);k++){
            cout << " ";
        }
        for (int j=0;j<(2*i+1);j++){
            cout << "*";
        }
        cout << endl;
    }
}
```
---
# Star Diamond
https://www.naukri.com/code360/problems/star-diamond_6573686?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems
![image](https://github.com/user-attachments/assets/9dafc855-6290-42bd-9e78-5f6856a62644)
### My original solution
```cpp
void nStarDiamond(int n) {
    for (int i=0;i<2*n;i++){
        if (i<n){
            for (int j=0;j<(n-i-1);j++)
                cout << " ";
            for (int k=0;k<(2*i+1);k++)
                cout << "*";
            cout << endl;
        }
        else {
            for (int j=0;j<(i-n);j++)
                cout << " ";
            for (int k=0;k<(4*n-2*i-1);k++)
                cout << "*";
            cout << endl;
        }
    }
}
```
### Optimized version
```cpp
void printDiamond(int n) {
    for (int i = 0; i < 2 * n; i++) {
        int spaces = (i < n) ? (n - i - 1) : (i - n);
        int stars  = (i < n) ? (2 * i + 1) : (4 * n - 2 * i - 1);
        cout << string(spaces, ' ') << string(stars, '*') << "\n";
    }
}
```
---
# Binary Number Triangle
https://www.naukri.com/code360/problems/binary-number-triangle_6581890?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems
![image](https://github.com/user-attachments/assets/d7265cd1-d2b8-435a-9842-7511d392e7ba)
### My solution
```cpp
void nBinaryTriangle(int n) {
    int start=1;
    for (int i=0;i<n;i++){
        if (i%2==0) start=1;
        else start=0;
        for (int j=0;j<=i;j++){
            cout << start << " ";
            start=1-start; //flips bits
        }
        cout << endl;
    }
}
```
# Number Crown
https://www.naukri.com/code360/problems/number-crown_6581894?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems
![image](https://github.com/user-attachments/assets/fc2fbbd6-19ad-40c7-b54b-8ab5137bfb79)
### My solution
```cpp
void numberCrown(int n) {
    for (int i=1;i<=n;i++){
        for (int j=1;j<=i;j++)
            cout << j << " ";
        cout << string(4*n-4*i,' ');
        for (int j=i; j>=1; j--)
            cout << j << " ";
        cout << endl;
    }
}
```




