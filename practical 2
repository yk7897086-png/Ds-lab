//linear search
#include <iostream>
using namespace std;

int main() {
    int n, key;
    int a[100];

    cout << "Enter number of elements: ";
    cin >> n;

    cout << "Enter elements:\n";
    for (int i = 0; i < n; i++) {
        cin >> a[i];
    }

    cout << "Enter key to search: ";
    cin >> key;

    for (int i = 0; i < n; i++) {
        if (a[i] == key) {
            cout << "Element found at index: " << i;
            return 0;
        }
    }

    cout << "Element not found";
    return 0;
}


//binary Search
#include <iostream>
using namespace std;

int main() {
    int n, key;
    int a[100];
    int low, high, mid;

    cout << "Enter number of elements: ";
    cin >> n;

    cout << "Enter elements in sorted order:\n";
    for (int i = 0; i < n; i++) {
        cin >> a[i];
    }

    cout << "Enter key to search: ";
    cin >> key;

    low = 0;
    high = n - 1;

    while (low <= high) {
        mid = (low + high) / 2;

        if (a[mid] == key) {
            cout << "Element found at index: " << mid;
            return 0;
        } 
        else if (a[mid] < key) {
            low = mid + 1;
        } 
        else {
            high = mid - 1;
        }
    }

    cout << "Element not found";
    return 0;
}