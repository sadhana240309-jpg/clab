#include <iostream>
#include <string>  // added
using namespace std;

class StudentRecord  // changed class name
{
private:
    int studentId;      // changed variable name
    string studentName; // changed variable name

public:
    // Constructor using initializer list
    StudentRecord(int r, string n) : studentId(r), studentName(n)
    {
        cout << "[Constructor] Record created for " << studentName << endl;
    }

    // Member function - renamed
    void showDetails()
    {
        cout << "Student ID: " << studentId << endl;
        cout << "Student Name: " << studentName << endl;
    }

    // Destructor
    ~StudentRecord()
    {
        cout << "[Destructor] Record for " << studentName << " destroyed" << endl;
    }
};

int main()
{
    // Your own test case
    StudentRecord s1(102, "Kumar");
    s1.showDetails();

    StudentRecord s2(103, "Priya");
    s2.showDetails();

    return 0;
}
