#include <iostream>
#include <cstdint>
using namespace std;

int main() {
	
	/*char s[10] = "hello\n";
	cout << s << endl;
	printf("%s", s); //%s - вывод строки
	//char s[] = { 'h','e','l','l','o' };
	for (size_t i = 0; i < 10; i++) {
		//printf("%d ", s[i]," "); //выводит кодировку s[i]
		//cout << int(s[i]) << endl;
	}
	char c = 88; // код в unicode 88  - X
	int j = 'X';
	cout << c << ' ' << j;
	int32_t x = 5;
	uint64_t y= 520;*/

	/*char s[256];
	cin.getline(s, 256);*/

	//двумерный массив
	/*int x[4][4];
	x[2][3] = 5;*/

	// массив из  указателей
	int m = 11, n = 11;
	int **a = new int*[n];
	for (int i = 0; i < m; i++) {
		a[i] = new int[n];
		for (int j = 0; j < n; j++) {
			a[i][j] = i * j;
		}

	}
	for (int i = 0; i < m; i++) {
		for (int j = 0; j < n; j++) {
			//cout << a[i][j] << '\t'; //  \t - табуляция
			printf("%4d", a[i][j]); // %4d - ширина 4
		}
		cout << endl;
	}

}
