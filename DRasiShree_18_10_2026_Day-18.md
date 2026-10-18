Code : Palindromic Times
```cpp
#include <bits/stdc++.h>
using namespace std;
int main() {
    string s;
    cin >> s;
    int hr = stoi(s.substr(0, 2));
    int mn = stoi(s.substr(3, 2));
    while (true) {
        int rev = (hr % 10) * 10 + hr / 10;
        if (rev > mn && rev < 60) {
            cout << (hr < 10 ? "0" : "") << hr << ":";
            cout << (rev < 10 ? "0" : "") << rev;
            return 0;
        }
        hr = (hr + 1) % 24;
        mn = -1;
    }
}
```
<img width="899" height="403" alt="image" src="https://github.com/user-attachments/assets/4f23781d-ed23-4745-b38e-0edd38f637fe" />
