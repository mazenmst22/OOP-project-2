# OOP-project-2
A Tiny project using OOP principles to get an info from user and print it (A Book information)
#include <iostream>
#include <string>
#include <vector>
#include <utility>
#include <cmath>
#include <cstdlib>
#include <algorithm>
using namespace std;

class Book {
private:
	string title;
	string author;
	int price;
public:
	Book(string t, string a, int p) {
		title = t;
		author = a;
		price = p;
	}
	string getTitle() {
		return title;

	}
	string getAuthor() {
		return author;
	}
	int getprice() {
		if (price > 0) {
			return price;
		}
	}

}; int main() {
	cout << "Enter Book details:(Title , Author , Price): ";
	string t; getline(cin, t);
	string a; getline(cin, a);
	int p; cin >> p;
	Book User1(t, a, p);
	cout << "The Book Title is: " << User1.getTitle() << endl;
	cout << "The Author is: " << User1.getAuthor() << endl;
	cout << "The Price is: " << User1.getprice() << endl;
	return 0;
}
