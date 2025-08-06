#include <iostream>
#include <string>
#include <direct.h>   
#include <windows.h>  

using namespace std;

void listFiles () {
    string pattern ;
        cout << "\nEnter file pattern (e.g., *.*, *.txt): ";
         cin >> pattern;
   }
   
  void mainMenu() {
    int choice;
    do {
        cout << "\n--- Directory Management System ---\n";
        cout << "[1] List Files\n[2] Create Directory\n[3] Change Directory\n[4] Exit\n";
        cout << "Choose an option: ";
        cin >> choice;

        switch (choice) {
            case 1: listFiles(); break;
            case 2: createDirectory(); break;
            case 3: changeDirectory(); break;
            case 4: cout << "Exiting program...\n"; break;
            default: cout << "Invalid choice.\n";
        }
    } while (choice != 4);
}
