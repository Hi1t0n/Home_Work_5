# Home_Work_5
/*Написать программу, которая находит сумму всех целых нечетных чисел в диапазоне, указанном пользователе.*/
#include <iostream>
using namespace std;
int main()
{
	setlocale(LC_ALL, "Russian");
	int min, max, sum;
	cout << "Введите начало диапозона чисел: ";
	cin >> min;
	cout << "Введите конец диапозона чисел: ";
	cin >> max;
	cout << "Сумма нечетных чисел в диапозоне от " << min << " до " << max << " равна: ";
	sum = 0;
	do
	{
		if (min % 2 != 0)
		{
			sum += min;
			
		}
		min++;

	} while (min <= max);
	cout << sum;

}

