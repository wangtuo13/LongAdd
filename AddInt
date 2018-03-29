#include <iostream>
#include <cstring>
using namespace std;
#define N 100

char a[100],b[100];
int sum[100]={0};
void show()
{
	int sig = 0;
	cout << "Result:  ";
	for (int i=N-1;i>=0;i--)
	{
		if (sum[i]>0)
		{
			sig = 1;
		}
		if (sig==1)
		{
			cout << sum[i];
		}
	}
}

void add()
{
	int jinwei = 0;
	int sigx=0;;
	int sigy=0;
	for (int i=0;i<N;i++)
	{
		if (a[i]=='\0')
		{
			sigx=1;
		}
		if (b[i]=='\0')
		{
			sigy=1;
		}
		int x,y,z ;
		x = (sigx==1) ? 0 : a[i] - '0';
		y = (sigy==1) ? 0 : b[i] - '0';
		z = x + y + jinwei;	
		sum[i] = z%10;
		jinwei = z/10;
	}
}

void write()
{
	cout << "Number1: ";
	cin >> a;
	cout << "Number2: ";
	cin >> b;
	strrev(a);
	strrev(b);
}

int main()
{
	write();
	add();
	show();
	return 0;
}
