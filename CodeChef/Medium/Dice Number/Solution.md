Here is the Solution of the Problem

```cpp
#include <iostream>
#include <vector>
#include <algorithm>
using namespace std;

int main() {
    int n;
    cin >> n;
    
    while (n--) {
        vector<int> v(6);

        for (int i = 0; i < 6; i++) {
            cin >> v[i];
        }

        vector<int> alice(v.begin(), v.begin() + 3);
        vector<int> bob(v.begin() + 3, v.end());

        sort(alice.begin(), alice.end(), greater<>());
        sort(bob.begin(), bob.end(), greater<>());

        if (alice > bob) {
            cout << "Alice" << endl;
        } else if (bob > alice) {
            cout << "Bob" << endl;
        } else {
            cout << "Tie" << endl;
        }
    }

    return 0;
}

```
