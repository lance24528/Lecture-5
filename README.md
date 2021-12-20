# Lecture-5
#include <iostream>
#include <string>
#include <iomanip>
#include <array>
#include <math.h>
using namespace std;
	
//Biography
#include <string>   
#include <iostream>
#include <math.h>
using namespace std;

int main() {

	string name, hTown; int age;
	cout << "Enter your first name: ";
	getline(cin, name);
	cout << "\nEnter your hometown: ";
	cin >> hTown;
	cout << "\nEnter your age: ";
	cin >> age;
	cout << "\n\nYour name is: " << name << " \n\nYou are from " << hTown << "\n\nAnd you are " << age << " years old \n";

}
//Temperature 1
int main() {
	
	double tempF;
	cout << "Temperature converter. Enter the temperature in Fahrenheit\n\n";
	cin >> tempF;
	double tempC = (tempF - 32) * 5 / 9;
	if (!cin.fail())
	{
		cout << "its " << tempC << "F";
	}
	else
	{
		cout << "\n\nInvalid Input try again";
	}
}
//Temperature 2
int main() {
	
	double tempC;
	cout << "Temperature converter. Enter the temperature in Fahrenheit\n\n";
	cin >> tempC;
	double tempF = (tempC * 9/5) + 32;
	if (!cin.fail())
	{
		cout << "its " << tempF << "C";
	}
	else
	{
		cout << "\n\nInvalid Input try again";
	}
}
 //Circles
 int main() {
	
	double radius;
	cout << "Circle area and circumference calculator.\n\n";
	cout << "Input the Radius of the circle: \n\n";
	cin >> radius;
	if (!cin.fail())
	{
		double area = 3.14 * pow(radius, 2); double circumference = 2 * 3.14 * radius;
		cout << "\nArea = " << area << "\nCircumference = " << circumference << endl;
	}
	else
	{
		cout << "\n\nInvalid input try again" << endl;
	}
}
  //Rectangle Triangle Square
  void square() {
	int side;
	cout << "\nInput the the length of one side of a square: ";
	cin >> side;
	double areaS = pow(side , 2);
	cout << "\nThe area of the Square is " << areaS << endl;
}
void triangle() {
	
	int baseT, heightT;
	cout << "\nInput the base of the triangle: ";
	cin >> baseT;
	cout << "\nInput the height of the triangle: ";
	cin >> heightT;
	double areaT = baseT & heightT / 2;
	cout << "The area of the Triangle is " << areaT << endl;
}
void rectangle() {

	double length, width;
	cout << "\nInput the length of rectangle: \n\n";
	cin >> length;
	cout << "\nInput the width of rectangle: \n\n";
	cin >> width;
	double areaR = length * width;
	cout << "The area of the Rectangle is " << areaR << endl;
}
int main() {
		
	int number;
	cout << "Area of a shape calculator. Please choose the number of chosen shape\n\n";
	cout << "1. Rectanngle\n2. Triangle\n3. Square\n\n";
	cin >> number;
	if (!cin.fail())
	{
		switch (number)
		{
		case 1:
			rectangle();
			break;
		case 2:
			triangle();
			break;
		case 3:
			square();
			break;
		default:
			cout << "\n\nInvalid Input. Try again" << endl;
			break;
		}		
	}
	else
	{
		cout << "\nInvalid Input. Try again" << endl;
	}
}
