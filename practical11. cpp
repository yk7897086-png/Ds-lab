#include <iostream>
#include <stack>
#include <sstream>
using namespace std;

// Function to check operator
bool isOperator(char ch) {
    return (ch == '+' || ch == '-' || ch == '*' || ch == '/');
}

// Function to perform operation
int performOperation(int a, int b, char op) {
    switch (op) {
        case '+': return a + b;
        case '-': return a - b;
        case '*': return a * b;
        case '/': return a / b;
    }
    return 0;
}

// Function to evaluate postfix expression
int evaluatePostfix(string exp) {
    stack<int> st;
    stringstream ss(exp);
    string token;

    while (ss >> token) {
        // If number
        if (!isOperator(token[0])) {
            st.push(stoi(token));
        }
        else {
            int val2 = st.top(); st.pop();
            int val1 = st.top(); st.pop();

            int result = performOperation(val1, val2, token[0]);
            st.push(result);
        }
    }

    return st.top();
}

int main() {
    // NOTE: Use space-separated postfix for multi-digit support
    string exp = "23 5 4 * + 9 -";

    cout << "Postfix Expression: " << exp << endl;
    cout << "Result: " << evaluatePostfix(exp) << endl;

    return 0;
}