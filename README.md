# Exercise-for-Functions

SLIDE 2

	#include <iostream>
	#include <string>
	#include <array>
	#include <math.h>
	using namespace std;

	string rootValues(double numB)
	{

		cout << "\nThe root from 1-10 is: " << endl;

		double numA = 1;

		do
		{
			cout << "[" << numA << "]" << " root value for " << numB << " is: ";
			double x = 1 / numA;
			double result = pow(numB, x);
			cout << result << endl;
			numA++;
		} while (numA != 11);

		return "\nThe code is completed.";

	}

	int main()
	{
		double number; //variable to store user response
		cout << "Enter a number: "; //ask the user for an input
		cin >> number; //get user input
		while (cin.fail()) //error handling
		{
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid input. Enter the number again: ";
			cin >> number;
		}

		//output string returned by function
		cout << rootValues(number);
	}

SLIDE 3

	#include <iostream>
	#include <string>
	#include <array>
	#include <math.h>
	using namespace std;

	string exponentValues(double numB)
	{
		cout << "\nThe exponent from 1-10 is: " << endl;

		double numA = 1;

		do
		{
			cout << "[" << numA << "]" << " exponent value for " << numB << " is: ";

			cout << pow(numB, numA) << endl;
			numA++;
		} while (numA != 11);

		return "\nThe code is completed.";

	}

	int main()
	{
		double number; //variable to store user response
		cout << "Enter a number: "; //ask the user for an input
		cin >> number; //get user input
		while (cin.fail()) //error handling
		{
			cin.clear();
			cin.ignore(1000, '\n');
			cout << "Invalid input. Enter the number again: ";
			cin >> number;
		}

		//output string returned by function
		cout << exponentValues(number);
	}
