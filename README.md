# S2-Jamela-Rose-Alcantara

    #include <iostream>
    #include <string>
    #include <math.h>
    using namespace std;

    int main()
    {
        string name;
        int num;
        int fac = 1, i = 1;
        int ans;

        cout << "Enter your full name: ";
        getline(cin, name);

        cout << "Enter a number: ";
        cin >> num;
        while (cin.fail()) 
        {
            cin.clear(); 
            cin.ignore(1000, '\n');
            cout << "Invalid input. Enter a number again: ";
            cin >> num;
        }

        cout << "\nFactorial: " << endl;
        do
        {
            fac = fac * i;
            i++;

        } while (i <= num);
        cout << fac << endl;

        cout << "\nTable from 10-1:" << endl;
        for (int x = 10; x >= 1; x--)
        {
            cout << num << "x" << x << "=" << num * x << endl;
        }

        cout << "\nExponent power from 10-5:" << endl;
        for (int y = 10; y >= 5; y--)
        {
            ans = (int) (pow(num, y));
            cout << num << "^" << y << " = " << ans << endl;
        }

        return 0;
    }
