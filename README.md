#include <iostream>

using namespace std;

int main() {
    int number;

    cout << "Please enter a 4-digit number: ";
    cin >> number;

    // Extract digits
    int lastDigit = number % 10;
    int firstDigit = number / 1000;

    // Display result
    cout << "Your yekan is: " << lastDigit << endl;
    cout << "Your hezargan is: " << firstDigit << endl;

    if (firstDigit == lastDigit) {
        cout << "You won!" << endl;
    } else {
        cout << "You lose." << endl;
    }

    return 0;
}
