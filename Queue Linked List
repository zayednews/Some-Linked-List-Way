#include <iostream>

using namespace std;
typedef struct node{
    char data;
    struct node *next;
}*nd;
nd front=NULL,rear=NULL;
void enqueue(char x)
{
    nd np=new node;
    np->data=x;
    np->next=NULL;
    if(rear==NULL)
    {
        front=np;
        rear=np;
    }
    else{
        rear->next=np;
        rear=np;
    }
}
char dequeue()
{
    if(front==NULL)
    {
        cout<<"Queue is empty";
        return 0;
    }
    else
    {
        char x=front->data;
        nd d=front;
        front=front->next;
        delete(d);
        return x;
    }
}
int main()
{
    enqueue('Z');
    enqueue('A');
    enqueue('Y');
    enqueue('E');
    enqueue('D');
    cout<<dequeue()<<" is deleted;";
    return 0;
}
