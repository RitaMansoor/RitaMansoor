#include <iostream> 
using namespace std;

int main(){
    
    int n, i, column, space;


    cout << "Enter the value of n: ";
    cin >> n;

    for(i = 0; i <= n; i++){

        for(space = 0; space < n - i; space++){
            cout << " ";
        }
        for(column = 0; column < 2 * i + 1; column++){
            cout << "*";
        }
        cout << endl; 
      
    }
    for(i = n + 1; i <= 2 * n; i++){
        for(space = 0 ; space < i - n; space++){
            cout << " ";
        }
        for(column = 0; column < 4 * n - 2 * i + 1; column++){
            cout << "*";
        }
        cout << endl;
    }

    return 0;
    
}
