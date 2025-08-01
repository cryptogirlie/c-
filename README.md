include <iostream>
#include <string>
using namespace std;

int main() {
    string texture;
    int quantity;
    int price = 0;

    cout << "Welcome to SheLovesScrunchies Official Website " << endl;
    cout << "Available textures:\n";
    cout << "- satin: 1000\n";
    cout << "- velvet: 1500\n";
    cout << "- silk: 2000\n";
    cout <<"-Ankara: 3500\n";

    cout << "Enter the texture you want: ";
    getline(cin, texture);

    cout << "How many do you want? ";
    cin >> quantity;

    if (texture == "satin") {price =1000;}
    else if (texture == "velvet") {price = 1500;}
    else if (texture == "silk") {price = 2000;}
    else if (texture == "ankara") {price = 3500;}
     else {
         cout << "Sorry, we don't have that texture " << endl;
         return 0;
     }

    int total = price * quantity;
    cout << "Total for " << quantity << " "  << texture << " scrunchie(s):" << total << endl;

    return 0;
}
