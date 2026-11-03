#include <iostream>
using namespace std;

// Abstract base class
class BaseShape
{
public:
    virtual float calculateArea() = 0; // Pure virtual function
    virtual ~BaseShape() {} // virtual destructor
};

// Derived class 1
class CircleShape : public BaseShape
{
private:
    float rad;

public:
    CircleShape(float r) : rad(r) {}

    float calculateArea() override
    {
        return 3.14f * rad * rad;
    }
};

// Derived class 2
class RectangleShape : public BaseShape
{
private:
    float len, wid;

public:
    RectangleShape(float l, float b) : len(l), wid(b) {}

    float calculateArea() override
    {
        return len * wid;
    }
};

// Derived class 3
class TriangleShape : public BaseShape
{
private:
    float b, h;

public:
    TriangleShape(float base, float height) : b(base), h(height) {}

    float calculateArea() override
    {
        return 0.5f * b * h;
    }
};

int main()
{
    // Your own test cases - changed values
    CircleShape c1(7);         // was 5
    RectangleShape r1(5, 8);   // was 4,6
    TriangleShape t1(12, 6);   // was 10,8

    BaseShape *shapePtr;

    shapePtr = &c1;
    cout << "Area of Circle is: " << shapePtr->calculateArea() << endl;

    shapePtr = &r1;
    cout << "Area of Rectangle is: " << shapePtr->calculateArea() << endl;

    shapePtr = &t1;
    cout << "Area of Triangle is: " << shapePtr->calculateArea() << endl;

    return 0;
}
