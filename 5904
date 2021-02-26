#include <iostream>
using namespace std;

void moo(int k, int len, int n) {
	if (n <= 3) {
		if (n == 1) cout << "m";
		else cout << "o";
		return;
	}
	int middle = (len - (3 + k)) / 2;
	
  if (n <= middle) return moo(k - 1, middle, n);
	if (n > middle + (3 + k)) return moo(k - 1, middle, n - (middle + (3 + k)));
	if (n == middle + 1) return moo(k, len, 1);
	if (n <= middle + (3 + k)) return moo(k, len, 2);
}

int main() {
	int n; cin >> n;
	int i, length = 0;
	for (i = 0; length <= n; i++) {
		length = 2 * length + (3 + i);

	}
	moo(i - 1, length, n);

}
