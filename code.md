'''C++
#include <iostream>
#include <vector>
using namespace std;
int main() {
 long n;
 cin >> n;
 vector<long> A(n);
 for (int i = 0; i < n; i++) {
 cin >> A[i];
 }
 for (int i = 1; i < n; i++) {
 if (A[i] < A[i - 1]) {
 cout << "-1" << endl;
 return 0;
 }
 }
 cout << A[n - 1] - A[0] << endl;
 return 0;
}
'''
