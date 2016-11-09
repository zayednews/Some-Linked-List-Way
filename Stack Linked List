#include <iostream>

using namespace std;

typedef struct node{
    char data;
    struct node *next;
}*nd;
nd top;

void push(char x)
{
    nd np=new node;
    np->data=x;
    np->next=top;
    top=np;
}
char pop()
{
    nd d=top;
    char x=top->data;
    top=top->next;
    delete(d);
    return x;
}
char tp()
{
    return (top->data);
}
bool ISEmpty()
{
    if(top==NULL)
    {
        cout<<"YES"<<endl;
        return true;
    }
    else
    {
        cout<<"NO"<<endl;
    return false;
    }
}
int main()
{
    top=NULL;
    push('Z');
    push('A');
    push('Y');
    push('E');
    push('D');
    cout<<pop()<<" is deleted"<<endl;;
    cout<<"Top element is "<<tp()<<endl;
    cout<<"Is your element empty??"<<endl;
    cout<<ISEmpty()<<endl;
    return 0;
}
