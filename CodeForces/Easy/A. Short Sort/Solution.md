## SOLUTION :
Here is the CPP code for the problem.

```cpp
#include <iostream>
#include <string>

using namespace std;

// Function to count inversions in a string
int countInversions(string s) {
    int inversions = 0;
    for (int i = 0; i < s.length(); i++) {
        for (int j = i + 1; j < s.length(); j++) {
            if (s[i] > s[j]) {
                inversions++;
            }
        }
    }
    return inversions;
}

int main() {
    int t;
    cin >> t; // Number of test cases

    while (t--) {
        string cards;
        cin >> cards; // Input the arrangement of cards

        int inversions = countInversions(cards);
        
        if (inversions <= 1) {
            cout << "YES" << endl;
        } else {
            cout << "NO" << endl;
        }
    }

    return 0;
}


```
Hope it helps. 😀
