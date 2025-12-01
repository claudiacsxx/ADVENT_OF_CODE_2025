# ADVENT_OF_CODE_2025
//DAY 1 - PROBLEMA 1

#include <iostream>
#include <string>
using namespace std;

int actual = 50;
int contador = 0;

void left(int rotation){
    actual = actual - rotation;
}

void right(int rotation){
    actual = actual + rotation;
}

void superior(){
    while(actual > 99){
        actual = actual - 100;
    }
}

void inferior(){
    while(actual < 0){
        actual = 100 + actual;
    }
}

int main(){
    actual = 50;
    contador = 0;

    string rotation;

    while(getline(cin, rotation)){
        if(rotation.empty()) continue;
        
        char first_letter = rotation[0];
        int numbers = stoi(rotation.substr(1));
        
        if(first_letter == 'L'){
            left(numbers);
        }
        else if(first_letter == 'R'){
            right(numbers);
        }
        superior();
        inferior();
        
        if(actual == 0 || actual == 100){
            contador++;
            cout << "*** HIT 0! Contador: " << contador << " ***" << endl;
        }
    }
    cout << "Contraseña: " << contador << endl;
    return 0;
}
