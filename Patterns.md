# Star triangle
https://www.naukri.com/code360/problems/star-triangle_6573671?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems&leftPanelTabValue=PROBLEM
![image](https://github.com/user-attachments/assets/752faa64-5d28-456d-a9a3-e9e8d60d67f3)  
### My solution
```cpp
void nStarTriangle(int n) {
    // Write your code here.
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
--------------------------------------------
# Reverse Star triangle
https://www.naukri.com/code360/problems/reverse-star-triangle_6573685?utm_source=youtube&utm_medium=affiliate&utm_campaign=striver_patternproblems&leftPanelTabValue=SUBMISSION
<img width="517" alt="Screenshot 2025-06-17 at 1 59 49 PM" src="https://github.com/user-attachments/assets/a8215890-3cc0-4549-b606-8ddd166a73cf" />  
### My solution
```cpp
void nStarTriangle(int n) {
    // Write your code here.
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
-------------------------------------------


