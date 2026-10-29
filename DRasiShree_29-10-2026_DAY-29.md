CODE : PHONE NUMBER
```cpp
#include <bits/stdc++.h>
using namespace std;
int main() {
    int n;
    string s;
    cin >> n >> s;
    if (n % 3 == 0) {
        for (int i = 0; i < n; i += 3) {
            cout << s.substr(i, 3);
            if (i + 3 < n) cout << "-";
        }
    }
    else if (n % 2 == 0) {
        for (int i = 0; i < n; i += 2) {
            cout << s.substr(i, 2);
            if (i + 2 < n) cout << "-";
        }
    }
    else {
        cout << s.substr(0, 3) << "-";
        for (int i = 3; i < n; i += 2) {
            cout << s.substr(i, 2);
            if (i + 2 < n) cout << "-";
        }
    }
}
```
<img width="810" height="405" alt="image" src="https://github.com/user-attachments/assets/67bf4ea1-562c-4e95-924d-83d7aad61cff" />
