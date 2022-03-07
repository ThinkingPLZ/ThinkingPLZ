#include <iostream>
using namespace std; 
int a = 1;
void Magic(int A[3][3])
{
	for (int i =0;i<3;i++)
	{
		for (int l = 0+i; l <= 2; l++)
		{
			 A[i][l] = a;
			 a++;
		}
	}
}
void Output(int A[3][3])
{
	for (int i = 0; i <= 2; i++)
	{
		for (int l = 0; l <= 2; l++)
		{
			if (A[i][l] ==0)
			{
				cout << " ";
			}
			else
			{
				cout << A[i][l];
			}
			
		}
		cout << endl;
	}
}
int main()
{

	int A[3][3] = {0};


	Magic(A);
	Output(A);

	return 0;
}
