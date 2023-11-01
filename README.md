#include <iostream>
using namespace std;
int evklid(int a,int b){
    if (a > b){
        a = a%b;
    }
    else{ b = b%a;}
    if ((a != 0) and (b!= 0)){
    evklid(a,b);}
    else {
        return a+b;
    }
}
int main() {
    int a,b;
    cout << "A:";
    cin >> a;
    cout << "B:";
    cin >> b;
    cout << "Result:"  << evklid(a,b);
}
