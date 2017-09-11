# movieTheater2
# created by me
#include<iostream>
#include<string>
#include<iomanip>
using namespace std;

int main()
{
	int adultTickets, childTickets;
	double grossBoxoffice, netBoxoffice, paidToDistributer;
	string movieName;

	cout << "Enter the movie name: " << endl;
	getline(cin,movieName);
	
	cout << "Enter number of adult tickets sold: " << endl;
	cin >> adultTickets;
	
	cout << "Enter number of child tickets sold: " << endl;
	cin >> childTickets;
	
	grossBoxoffice = (adultTickets * 10.00) + (childTickets * 6.00);
	//cout << grossBoxoffice <<endl;
	
	netBoxoffice = (grossBoxoffice * 0.20);
	
	//cout << netBoxoffice <<endl;
	paidToDistributer = (grossBoxoffice - netBoxoffice);
	
	//cout << paidToDistributer << endl;
	cout << fixed << setprecision(2);
	cout << "REVENUE REPORT" << endl;
	cout << "==============" << endl;
	cout << "Movie Name: " << setw(43) << movieName << endl;
	cout << "Adult Tickets Sold: " << setw(29) << adultTickets << endl;
	cout << "Child Tickets Sold: " <<setw(29) << childTickets << endl;
	cout << "Gross Box Office Profit: " << setw(17) <<"$"<<grossBoxoffice << endl;
	cout << "Net Box Office Profit: " << setw(20) <<"$"<<netBoxoffice << endl;
	cout << "Amount paid to distributer: " << setw(14) <<"$"<< paidToDistributer << endl;
		
	system("pause");
}
