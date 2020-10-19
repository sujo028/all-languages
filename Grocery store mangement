#include<iostream.h>
#include<conio.h>
#include<stdio.h>
#include<ctype.h>
#include<stdlib.h>
const int m=10;

class ITEM
{
   int itemcode[m];
   float itemprice[m];
   int count;
 public:
	 void cntini(void)
	 {
	   count=0;
	 }

     void additem(); //add an item.
     void largest();//largest item price.
     void remove(); //to remove an item.
     void dispsum(); //to display total.
     void dispitem();  //to display items.
};

 void ITEM::additem(void)
 {
    char c='y';
    int i=count;
    do
    {
       cout<<"Item Number:"<<(i+1);
       cout<<"\n Enter Item Code:";
       cin>>itemcode[i];
       cout<<"\nItem Price:";
       cin>>itemprice[i];
       i++;
       count=i;
	if(i>=m)
	{
	    cout<<"\nNo more addition of item po9ssible:";
	    break;
	}
      cout<<"\nContinue(y/n)?:";
      cin>>c;
  }
   while(tolower(c)=='y');
} //function ends.

  void ITEM::largest(void)  //largest price.;
  {
    float large=itemprice[0];
    int laritcode=itemcode[0];
    for(int i=1;i<count;i++)
       if(large<itemprice[i])
       {
	 large=itemprice[i];
	 laritcode=itemcode[i];
       }
     cout<<"\nLargest Price Item \n";
     cout<<laritcode<<"\t"<<large;
   }//function ends.

 void ITEM::remove(void)//to remove an item.
 {
    int a;
    cout<<"\nEnter Item Code:";
    cin>>a;
     for(int i=0;i<count;i++)
	 if(itemcode[i]==a)
	    itemprice[i]=0;
     cout<<"\nDelected....****";
  }//function ends.

   void ITEM::dispsum(void) //to display total.
   {
      float sum=0;
      for(int i=0;i<count;i++)
	  sum=sum+itemprice[i];
      cout<<"\nTotal Price:"<<sum<<endl;
   }//function ends.

  void ITEM::dispitem(void) //to display selected item.
  {
      cout<<"\n Code\t\t\tPrice";
      for(int i=0;i<count;i++)
	  cout<<"\n"<<itemcode[i]<<"\t\t\t"<<itemprice[i];
  }//fuinction ends.

  void main()
   {
      ITEM order;
      order.cntini();
      int choice;
      do
      {
	 //system("cls");
	 cout<<"\nShopping Cart Menu :";
	 cout<<"\n1.Addtion item"<<endl;
	 cout<<"2.Display total Price"<<endl;
	 cout<<"3.Display largest price."<<endl;
	 cout<<"4.Display all item."<<endl;
	 cout<<"5.Remove on  item"<<endl;
	 cout<<"6.EXIT."<<endl;
	 cout<<"Enter your choice(1-6):";
	 cin>>choice;
	 switch(choice)
	 {
	    case 1:order.additem();break;
	    case 2:order.dispsum();break;
	    case 3:order.largest();break;
	    case 4:order.dispitem();break;
	    case 5:order.remove();break;
	    case 6:break;
	    default:cout<<"\nWRONG OPTION****////";break;
	 }

       cout<<"\nPress any key to continue.";
       getch();
    }
   while(choice!=6);
 }//main ****.




