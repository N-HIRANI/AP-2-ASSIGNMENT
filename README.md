# AP-2-ASSIGNMENT
APPLICATION PROGRAMMING 2 ASSIGNMENT


NAMAN RAJENDRA HIRANI
SCT221-C002-0019/2021
BIT 3.2
APPLICATION PROGRAMMING 2



QUESTION ONE
#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    srand(time(0));
    int n = rand() % 200 - 100;
    if (n > 0)
        std::cout << "The number is positive";
    else if (n < 0)
        std::cout << "The number is negative";
    else
        std::cout << "The number is zero";
    return 0;
}


QUESTION TWO
#include <iostream>
#include <cstdlib>
#include <ctime>

int main() {
    srand(time(0));
    int n = rand() % 200 - 100;
    std::cout << "The last digit is " << abs(n) % 10;
    return 0;
}


QUESTION THREE
#include <iostream>

void swap(int &a, int &b) {
    int temp = a;
    a = b;
    b = temp;
}



QUESTION FOUR
#include <iostream>
#include <string>

void print_string(const std::string &s) {
    std::cout << s << std::endl;
}


QUESTION FIVE
#include <iostream>
#include <string>
#include <algorithm>

void print_reverse(std::string s) {
    std::reverse(s.begin(), s.end());
    std::cout << s << std::endl;
}

QUESTION SIX
#include <iostream>
#include <string>

size_t prefix_length(const std::string &s, const std::string &prefix) {
    if (s.substr(0, prefix.size()) == prefix)
        return prefix.size();
    else
        return 0;
}

