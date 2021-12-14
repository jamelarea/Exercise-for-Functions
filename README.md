# Exercise-for-Functions

SLIDE 2

    #include <iostream>
    #include <string>
    #include <array>
    #include <math.h>
    using namespace std;

    string rootValues(double n)
    {

      for (int i(10); i > 0; i--)
      {
        double powValue = (1.0 / i);
        cout << n << " to the root of " << i << " is: " << pow(n, powValue) << endl;
      }
      
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

	string exponentValues(double n)
	{

		for (int i(10); i > 0; i--)
		{
			double result = pow(n, i);
			cout << n << "^" << i << " is: " << result << endl;
		}

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
