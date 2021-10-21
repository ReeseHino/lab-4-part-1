# lab-4-part-1
#include <iostream>
#include <iomanip>
#include <cmath>
using namespace std;

int main()
{
  double mass;
  double accelEarth = 9.81
  double accelMoon = 1.62;
  double accelVenus = 8.87;

  cout << "Enter the mass in kg" << endl;
    cin >> mass;
      if (mass <= 0) {
        cout << fixed << setprecision (4); 
        cout << "The mass is " << mass << " kg" << endl;
        cout << "The mass must be greater than zero" << endl;
        }
      else {
        cout << fixed << setprecision (4); 
        cout << "The mass is " << mass << " kg" << endl;
        cout << left << setw(8) << "Location";
        cout << right << setw(14) << "Weight (N)" << endl;

        double weigthONearth = mass * accelEarth;

        cout << left << setw(8) << "Earth" << right << setw(14) << weightONearth << endl;
        cout << left << setw(8) << "Moon" << right << setw(14) << mass * accelMoon << endl;
        cout << left << setw(8) << "Venus" << right << setw(14) << mass* accelVenus << endl;

          if (weightONearth <= 1500) {
            cout << "The object is heavy" << endl;
            }
          if (weightONearth < 5) {
            cout << "The object is light" << endl;
            }
        
          }
   return 0;
}
