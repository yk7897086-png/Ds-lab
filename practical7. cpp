#include <iostream>
using namespace std;

struct Node {
    int data;
    Node* next;
};

Node* head = NULL;

// Create (Insert at end)
void create(int x) {
    Node* newNode = new Node();
    newNode->data = x;
    newNode->next = NULL;

    if (head == NULL)
        head = newNode;
    else {
        Node* temp = head;
        while (temp->next != NULL)
            temp = temp->next;
        temp->next = newNode;
    }
}

// Insert at beginning
void insertBegin(int x) {
    Node* newNode = new Node();
    newNode->data = x;
    newNode->next = head;
    head = newNode;
}

// Delete from beginning
void deleteBegin() {
    if (head == NULL) {
        cout << "List is empty\n";
        return;
    }
    Node* temp = head;
    head = head->next;
    delete temp;
}

// Traversal
void display() {
    Node* temp = head;
    while (temp != NULL) {
        cout << temp->data << " -> ";
        temp = temp->next;
    }
    cout << "NULL\n";
}

int main() {
    create(10);
    create(20);
    create(30);

    cout << "List: ";
    display();

    insertBegin(5);
    cout << "After insertion: ";
    display();

    deleteBegin();
    cout << "After deletion: ";
    display();

    return 0;
}