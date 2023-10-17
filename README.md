#include <iostream>
#include <cstdlib>
#include <ctime>
#include <wchar.h>
#include <Windows.h>
#include <algorithm>
#include <vector>
#include <string>
#include <conio.h>
#include <iomanip>



using namespace std;
const int SIZE = 4;
struct part {
    int modelnumber;
    int partnumber;
    float cost;
};


int main()
{
    int n;
    part apart[SIZE];

    for (n = 0; n < SIZE; n++) {
        cout << endl;
        cout << "Enter the model number: ";
        cin >> apart[n].modelnumber;
        cout << "Enter the part number: ";
        cin >> apart[n].partnumber;
        cout << "Enter the price: ";
        cin >> apart[n].cost;
    }
    cout << endl;
    for (n = 0; n < SIZE; n++) {
        cout << "Model " << apart[n].modelnumber;
        cout << "Part " << apart[n].partnumber;
        cout << "cost " << apart[n].cost;
    }
    
    

    return 0;
}
