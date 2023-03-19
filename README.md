# itsa-no.11
#include <iostream>
using namespace std;

  
  
int main() {  
    const int MAX_SIZE = 100;  
    int arr[MAX_SIZE], n;  
    cout << "請輸入組數長度（不超過" << MAX_SIZE << "）：";  
    cin >> n;  
    cout << "請輸入" << n << "個整數，用空格隔開：";  
    for (int i = 0; i < n; i++) {  
        cin >> arr[i];  
    }  
    cout << "反轉前的數組為：";  
    for (int i = 0; i < n; i++) {  
        cout << arr[i] << " ";  
    }  
    cout << endl;  
    for (int i = 0; i < n / 2; i++) {  
        int temp = arr[i];  
        arr[i] = arr[n - i - 1];  
        arr[n - i - 1] = temp;  
    }  
    cout << "反轉後的數組為：";  
    for (int i = 0; i < n; i++) {  
        cout << arr[i] << " ";  
    }  
    cout << endl;  
    return 0;  
}

