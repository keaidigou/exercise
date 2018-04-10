
###### exercise1
```
把一個陣列全部都平方
改自教科書範例
```
```
#include <iostream>
using namespace std;

int main()
{
  const int NUMBER_OF_ELEMENTS = 5;
  double numbers[NUMBER_OF_ELEMENTS];
  double numbers_spure[NUMBER_OF_ELEMENTS];
  double sum = 0;

  for (int i = 0; i < NUMBER_OF_ELEMENTS; i++)
  {
    cout << "Enter a new number: ";
    cin >> numbers[i];
    sum += numbers[i];
    numbers_spure[i]=numbers[i]*numbers[i];
  }

  double average = sum / NUMBER_OF_ELEMENTS;

  int count = 0; // The number of elements above average
  for (int i = 0; i < NUMBER_OF_ELEMENTS; i++)
    if (numbers[i] > average)
      count++;

  cout << "Average is " << average << endl;
  
  cout<<"numbers[0] is "<<numbers[0]<<endl;
  
  cout<<"numbers[1] is "<<numbers[1]<<endl;
  
  cout<<"numbers[2] is "<<numbers[2]<<endl;
  
  cout<<"numbers[3] is "<<numbers[3]<<endl;
  
  cout<<"numbers[4] is "<<numbers[4]<<endl;
  
  cout << "Number of elements above the average " << count << endl;
  system ("pause");
  return 0;
}
```
```
說明:
numbers_squared[i]=numbers[i]*numbers[i];


```
###### exercise2

```
