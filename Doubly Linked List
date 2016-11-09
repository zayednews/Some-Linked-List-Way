#include <iostream>

using namespace std;
typedef struct node{
    char data;
    struct node *next,*prev;
}*nd;
nd start,end,np,p;

void insert(int x)
{
    np = new node;
    np->data=x;
    np->next=NULL;
    np->prev=NULL;
if(start==NULL){
	start=np;
	end=np;
	}
	else{

	    np->next=start;
	    start->prev=np;
	    start=np;
	}
	//p=np;
}
void display()        //displaying
{

    nd temp3=start;
    if(start==NULL)
        cout<<"no node to display"<<endl;
    else
    {
      while(temp3->next!=NULL)
      {
          cout<<"Data stored is "<<temp3->data<<" at "<<temp3<<endl;
         temp3=temp3->next;
      }
      cout<<"Data stored is "<<temp3->data<<" at "<<temp3<<endl;
    }
}
void rev_display()        //displaying
{

    nd temp3=start;
    if(start==NULL)
        cout<<"no node to display"<<endl;
    else
    {
      while(end->prev!=NULL)
      {
          cout<<"Data stored is "<<end->data<<" at "<<temp3<<endl;
         end=end->prev;
      }
      cout<<"Data stored is "<<end->data<<" at "<<temp3<<endl;
    }
}

int main()
{
    start=NULL;
end=NULL;
insert('Z');
insert('A');
insert('Y');
insert('E');
insert('D');
display();
rev_display();
//    cout << " "<<< endl;

    return 0;
}
