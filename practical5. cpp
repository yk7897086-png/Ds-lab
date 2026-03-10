#include<iostream>
using namespace std;

#define SIZE 5

int queue[SIZE];
int front = -1;
int rear = -1;

void enqueue(int value)
{
    if(rear == SIZE-1)
    {
        cout<<"Queue Overflow"<<endl;
    }
    else
    {
        if(front == -1)
            front = 0;

        rear++;
        queue[rear] = value;

        cout<<"Inserted: "<<value<<endl;
    }
}

void dequeue()
{
    if(front == -1 || front > rear)
    {
        cout<<"Queue Underflow"<<endl;
    }
    else
    {
        cout<<"Deleted: "<<queue[front]<<endl;
        front++;
    }
}

void peek()
{
    if(front == -1 || front > rear)
    cout<<"Queue is Empty"<<endl;

    else
    cout<<"Front Element: "<<queue[front]<<endl;
}

void isEmpty()
{
    if(front == -1 || front > rear)
    cout<<"Queue is Empty"<<endl;

    else
    cout<<"Queue is Not Empty"<<endl;
}

void isFull()
{
    if(rear == SIZE-1)
    cout<<"Queue is Full"<<endl;

    else
    cout<<"Queue is Not Full"<<endl;
}

void size()
{
    if(front == -1 || front > rear)
    cout<<"Queue size: 0"<<endl;

    else
    cout<<"Queue size: "<<rear-front+1<<endl;
}

void display()
{
    if(front == -1 || front > rear)
    {
        cout<<"Queue is Empty"<<endl;
    }
    else
    {
        cout<<"Queue Elements: ";
        for(int i=front;i<=rear;i++)
        cout<<queue[i]<<" ";

        cout<<endl;
    }
}

int main()
{
    int choice,value;

    while(true)
    {
        cout<<"\n1.Enqueue";
        cout<<"\n2.Dequeue";
        cout<<"\n3.Display";
        cout<<"\n4.Peek";
        cout<<"\n5.isEmpty";
        cout<<"\n6.isFull";
        cout<<"\n7.Size";
        cout<<"\n8.Exit";

        cout<<"\nEnter Choice: ";
        cin>>choice;

        switch(choice)
        {
            case 1:
            cout<<"Enter Value: ";
            cin>>value;
            enqueue(value);
            break;

            case 2:
            dequeue();
            break;

            case 3:
            display();
            break;

            case 4:
            peek();
            break;

            case 5:
            isEmpty();
            break;

            case 6:
            isFull();
            break;

            case 7:
            size();
            break;

            case 8:
            return 0;

            default:
            cout<<"Invalid Choice";
        }
    }
}