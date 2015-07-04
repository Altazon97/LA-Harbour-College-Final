//LA Harbour College - C++ Final by Eric Sund

#include <iostream>
using namespace std;

int choice;
int process = 1;
float total = 0;
//Giving variables to the properties of the items
//Stock
int pants_quant = 11;
int tshirt_quant = 4;
int jacket_quant = 5;
int sweater_quant = 22;
int jeans_quant = 9;
int boots_quant = 28;

//Stock in the shopping cart
int shop_pants_quant = 0;
int shop_tshirt_quant = 0;
int shop_jacket_quant = 0;
int shop_sweater_quant = 0;
int shop_jeans_quant = 0;
int shop_boots_quant = 0;

//Prices
float pants_price = 49.99;
float tshirt_price = 8.83;
float jacket_price = 29.99;
float sweater_price = 22.5;
float jeans_price = 37;
float boots_price = 39.19;

//Prices in Shopping Cart
float shop_jeans_price = 0;
float shop_boots_price = 0;
float shop_sweater_price = 0;
float shop_jacket_price = 0;
float shop_tshirt_price = 0;
float shop_pants_price = 0;

int main()
{
	while (process == 1)
	{
		cout<<"\n\n1. Print available items";
		cout<<"\n2. Add item to cart";
		cout<<"\n3. Print receipt and quit";
		cout<<"\nPlease enter your choice: ", cin>>choice;

			
		if (choice != 1 && choice != 2 && choice != 3)
		{
			cout<<"\nERROR! Insufficient quantity available. Please try again.";
		}
	
		if (choice == 1)
		{
			cout<<"\n\nDescription     Quantity                   Price";
			cout<<"\n  1) Pants       "<<pants_quant  << " left   $" << pants_price;
			cout<<"\n  2) T-Shirt     "<<tshirt_quant << " left   $" << tshirt_price << " ON SALE! reg. $10.15";
			cout<<"\n  3) Jacket      "<<jacket_quant << " left   $" << jacket_price;
			cout<<"\n  4) Sweater     "<<sweater_quant<< " left   $" << sweater_price;
			cout<<"\n  5) Jeans       "<<jeans_quant  << " left   $" << jeans_price;
			cout<<"\n  6) Boots       "<<boots_quant  << " left   $" << boots_price << " ON SALE! reg. $41.25";
		}

		if (choice == 2)
		{
			int item;
			int quant;
			cout<<"\n\nPlease enter the item to add and quantity to add: ";
			cin>>item>>quant;
			if (item == 1)
			{
				pants_quant -= quant;
				shop_pants_quant += quant;
				shop_pants_price = shop_pants_quant * pants_price;
			}
			if (item == 2)
			{
				tshirt_quant -= quant;
				shop_tshirt_quant += quant;
				shop_tshirt_price = shop_tshirt_quant * tshirt_price;
			}
			if (item == 3)
			{
					jacket_quant -= quant;
				shop_jacket_quant += quant;
				shop_jacket_price = shop_jacket_quant * jacket_price;
			}
			if (item == 4)
			{
				sweater_quant -= quant;
				shop_sweater_quant += quant;
				shop_sweater_price = shop_sweater_quant * sweater_price;
			}
			if (item == 5)
			{		
				jeans_quant -= quant;
				shop_jeans_quant += quant;
				shop_jeans_price = shop_jeans_quant * jeans_price;
			}
			if (item == 6)
			{
				boots_quant -= quant;
				shop_boots_quant += quant;
				shop_boots_price = shop_boots_quant * boots_price;
			}
		}

		if (choice == 3)
		{
			float total = shop_jeans_price + shop_boots_price + shop_sweater_price + shop_jacket_price + shop_tshirt_price + shop_pants_price;
			cout<<"\n\nRECEPT:\n";
			cout<<shop_pants_quant << "    x Pants    " << pants_price << " ea.\n";
			cout<<shop_tshirt_quant << "    x T-Shirt  " << tshirt_price << " ea.\n";
			cout<<shop_jacket_quant << "    x Jacket   " << jacket_price << " ea.\n";
			cout<<shop_sweater_quant << "    x Sweater  " << sweater_price << " ea.\n";
			cout<<shop_jeans_quant << "    x Jeans    " << jeans_price << " ea.\n";
			cout<<shop_boots_quant << "    x Boots    " << boots_price << " ea.\n";
			cout<<"\n---------------------------------------------------------------------------";
			cout<<"\n$" << total;
			//The program exits immidiately after it gets to the next line.  You might want to put in something that says "press anything to exit" but
			//I'm not sure if that follows criteria.
			process = 0;
		}
	}
	return 0;
}