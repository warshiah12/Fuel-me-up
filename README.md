# Fuel-me-up
Diesel or petrol
#include<iostream>
using namespace std;
int main()
{
	char fuel;
	double litres;
	int price;
	char ch;
	cout << "Fuel Type? Enter p for petrol and d for diesel : " << endl;
	cin >> fuel;
	cout << "Enter Litres: " << endl;
	cin >> litres;
	if (litres != 0)  //if litre is not equal to 0 then the control will be transfered to the switch statement else it will move to else statement  
	{
		switch (fuel)
		{
		case 'P':   //if the user enters capital or small p then the following statement will be executed 
		case'p':

			cout << "You have selected petrol. \nRate per litre is 0.8" << endl;
			price = litres * 0.8;
			cout << price << " AED " << endl;
			break;
		case 'D':   //if the user enters capital or small d then the following statement will be executed 
		case 'd':
			cout << "You have selected diesel. \nRate of diesel is 0.9" << endl;
			price = litres * 0.9;
			cout << price << " AED " << endl;
			break;
		default:   //if the user enters any other letter except 'p' and 'd' then the following statement will be executed 
			cout << "You entered invalid fuel type..." << endl;
			break;
		}
	}
	else
	{
		cout << "Invalid input" << endl;
	}
		return 0;
}
