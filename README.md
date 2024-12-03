# Ovsiyenko_lab8

#include <iostream>
#include <string>

bool arePalindromes(const std::string& str1, const std::string& str2) {
    if (str1.size() != str2.size()) {
        return false;
    }

    for (size_t i = 0; i < str1.size(); ++i) {
        if (str1[i] != str2[str2.size() - 1 - i]) {
            return false;
        }
    }

    return true;
}

int main() {
    
    std::string str1 = "abc";
    std::string str2 = "cba";

    std::cout << (arePalindromes(str1, str2) ? "Так" : "Ні") << std::endl;

    return 0;
}
