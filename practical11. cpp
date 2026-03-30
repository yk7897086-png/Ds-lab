#include <iostream>
#include <vector>
using namespace std;

class Graph {
    int V;
    vector<int>* adj;

public:
    Graph(int V) {
        this->V = V;
        adj = new vector<int>[V];
    }

    // Add edge
    void addEdge(int u, int v) {
        adj[u].push_back(v);
        adj[v].push_back(u); // remove this line for directed graph
    }

    // Display graph
    void display() {
        for (int i = 0; i < V; i++) {
            cout << i << " -> ";
            for (int j = 0; j < adj[i].size(); j++) {
                cout << adj[i][j] << " ";
            }
            cout << endl;
        }
    }
};

int main() {
    Graph g(4);

    g.addEdge(0, 1);
    g.addEdge(0, 2);
    g.addEdge(1, 3);
    g.addEdge(2, 3);

    cout << "Adjacency List:\n";
    g.display();

    return 0;
}