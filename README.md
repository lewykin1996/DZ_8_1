# DZ_8_1 (Считающая функция)

#include <iostream>
#include <string>
#include <math.h>

using namespace std;



void counting_function()
{
	static int x = 0;
	x++;
	cout << "Количество вызовов функции counting_function(): " << x << endl;
}

int main(int argc, char** argv)
{
	setlocale(LC_ALL, "Russian");

	for (int i = 0; i < 15; i++)
	{
		counting_function();
	}
}

