# master4.0
#include <iostream>
using namespace std;
int x, y;
int r=0 ;
void sum (int x, int y)
{
  while (x<=y)
  {
    r=r+x;
    x++;
  }
}
int main ()
{
  cout<<"We will calculate the sum of integers in the range you provide"<< endl;
  cout<<"Please enter lower bound:"; cin>> x;
  cout <<"Please enter upper bound:"; cin>>y;
  if (x<=y)
  {
    sum (x,y);
  }
  else
  {
    cout<<"This is not the way you should do that, we need to change the bounds around, and now it works.";
    sum (y,x);
  }
  cout<< endl;
    cout<<"The sum is:"<< r << endl;
    return 0;
}
