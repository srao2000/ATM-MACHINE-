# ATM-MACHINE-
#include<iostream>
#include<bits/stdc++.h>
using namespace std;
void printstar(char ch , int n);
double balance1;
int main()
{
system("color 70");
cout<<"\n\t\t ========================================="<< endl;
cout<<"\t\t ========================================="<< endl;
cout<<"\t\t      || WELCOME TO ATM MACHINE ||     "<< endl;
cout<<"\t\t ========================================="<< endl;
cout<<"\t\t ========================================\n\n"<< endl;
printstar('*',80);
int pin;
string id ;
/*'SANJEEV',"PANKAJ","RAVINDER","YOGITA";
map<string,long long int>m;
m[SANJEEV]=5555;
m[PANKAJ]=6666;
m[RAVINDER]=7777;
m[YOGITA]=8000;
bool pinchange()
{
	cout<<"ENTER YOUR ID ";
	string name;
	cin>>name;
	cout<<"ENTER YOUR OLD PIN";
	long long old,new_pin;
	cin>>old;
	if(m[name]==old)
	{
		cout<<"ENTER YOUR NEW PIN";
		cin>>new_pin;
		m[name]=new_pin;
		return 1;
	}
	return 0;
}*/
cout<<" ************** PIN CODE FOR SANJEEV IS 5555 **************\n";
cout<<" ************** PIN CODE FOR PANKAJ IS 6666 ************** \n";
cout<<" ************** PIN CODE FOR RAVINDER IS 7777 ************** \n";
cout<<" ************** PIN CODE FOR YOGITA IS 8888 ************** \n\n\n";
printstar('&',80);
for(int i=1;i<=10;i++)
{
  // if(i==2 || i==3 || i==4 || i==5 || i==6 || i==7 || i==8 || i==9 || i==10)
      cout<<"\n\t\t\t WELCOME TO YADAV BANK \n\t\t\t\t MAIN PAGE \n";     
   cout<<"PLEASE ENTER THE ID in capital letter\n";
   cin>>id;
   //system("cls");
   if(id == "SANJEEV")
    {
       cout<<"\n WELCOME Mr SANJEEV \n";
       for (int i=0;i<3;i++)
         {
           cout <<"enter pin:\n";
           cin>>pin;
           double balance = 10000;
           balance1=balance;
           if (pin==5555)
             {
               for(int i=1;i<=10;i++)
                {
                  double withdraw, deposit;
                  int option;
                  cout<<"\n";
                  if(i==1)
                   {
                      cout<<"\t\t *** Automated Teller Machine ***"<< endl;
                      cout<<"\nChoose a Transaction:\n\n";
                   }
                  printstar('%',80);
                  cout<<" MAIN SCREEN \n";
                  cout<<"[1] Inquire Balance \n";
                  cout<<"[2] Withdraw \n";
                  cout<<"[3] Deposit \n";
                  cout<<"[4] Quit \n";
                  cout<<"\n";
                  cout<<"Enter Option:";
                  cin>>option;
                  switch(option)
                   {
                     case 1:
                        cout<<"\n[[[% BALANCE INQUIRY %]]]\n";
                        cout<<"\n Your current balance is RS "<< balance1<< endl;
                        continue;
                     case 2:
                        cout<<"\n[[[% WITHDRAW %]]]\n";
                        cout<<"Enter amount in Rupees: ";
                        cin>>withdraw;
                        balance1 = balance1 - withdraw;
                        cout<<"You withdrew RS: "<< withdraw<< endl;
                        cout<<"Your remaining balance is RS: "<< balance1<< endl;
                        continue;
                     case 3:
                        cout<<"\n[[[% DEPOSIT %]]]\n";
                        cout<<"Enter amount in RS: ";
                        cin>>deposit;
                        balance1 = balance1 + deposit;
                        cout<<"You deposited RS: "<< deposit<< endl;
                        cout<<"Your new balance is RS: "<< balance1<< endl;
                        continue;
                    case 4:
                        cout<<"\n***[[[% EXIT MODE %]]]***\n";
                        system("cls");
                        break;
                    default:
                        cout<<"\n That is an invalid option Plz enter correct option: \n";
                         continue;
                  }
                 break;
               }
           break;
          } 
        else if(i==2)
         {
           cout<<"\nCard is captured\n";
         }
       else
          cout<<"Pls try again!!!\n";
          
    }
}
    if(id == "PANKAJ")
     {
        cout<<"\n WELCOME Mr PANkAJ \n";
        for (int i=0;i<3;i++)
         {
           cout <<"enter pin:\n";
           cin>>pin;
           double balance = 52000;
           balance1=balance;
           int flag=1;
           if (pin==6666)
            {
              for(int i=1;i<=10;i++)
                {
                  double withdraw, deposit;
                  int option;
                  cout<<"\n";
                  if(i==1)
                    {
                      cout<<"*** Automated Teller Machine***"<< endl;
                      cout<<"Choose a Transaction:\n";
                      cout<<"\n";
                    }
                    cout<<" MAIN SCREEN \n";
                    cout<<"[1] Inquire Balance \n";
                    cout<<"[2] Withdraw \n";
                    cout<<"[3] Deposit \n";
                    cout<<"[4] Quit \n";
                    cout<<"\n";
                    cout<<"Enter Option:";
                    cin>>option;
                    switch(option)
                     {
                       case 1:
                         cout<<"\n[[[% BALANCE INQUIRY %]]]\n";
                         cout<<"\n Your current balance is RS: "<< balance1<< endl;
                         continue;
                       case 2:
                         cout<<"\n[[[% WITHDRAW %]]]\n";
                         cout<<"Enter amount RS: ";
                         cin>>withdraw;
                         balance1 = balance1 - withdraw;
                         cout<<"You withdrew RS: "<< withdraw<< endl;
                         cout<<"Your remaining balance is RS: "<< balance1<< endl;
                         continue;
                       case 3:
                         cout<<"\n[[[% DEPOSIT %]]]\n";
                         cout<<"Enter amount RS: ";
                         cin>>deposit;
                         balance1 = balance1 + deposit;
                         cout<<"You deposited RS"<< deposit<< endl;
                         cout<<"Your new balance is RS: "<< balance1<< endl;
                         continue;
                       case 4:
                          cout<<"\n***[[[EXIT MODE]]]***\n";
                          flag=0;
                          break;
                       default:
                          cout<<"\n That is an invalid option Plz enter correct option:\n";
                          continue;
                     }
                if(flag==0)   
                   break;
                }
            }
          //  cout<<i<<endl;
          if(flag=0)      
             break;
     if(i==1)
       {
          cout<<"\nCard is captured\n";
       }
     else
          cout<<"Pls try again!!!\n";
      
   }
 }
    else if(id == "RAVINDER")
      {
         cout<<"\n Wellcome Mr RAVINDER \n";
         for (int i=0;i<3;i++)
          {
            cout <<"Please enter pin:\n";
            cin>>pin;
            double balance = 10000;
            balance1=balance;
            if (pin==7777)
             {
               for(int i=1;i<=10;i++)
                {
                  double withdraw, deposit;
                  int option;
                  cout<<"\n";
                  if(i==1)
                   {
                      cout<<"*** Automated Teller Machine***"<< endl;
                      cout<<"Choose a Transaction:\n";
                      cout<<"\n";
                   }
                   cout<<" MAIN SCREEN \n";
                   cout<<"[1] Inquire Balance \n";
                   cout<<"[2] Withdraw \n";
                   cout<<"[3] Deposit \n";
                   cout<<"[4] Quit \n";
                   cout<<"\n";
                   cout<<"Enter Option:";
                   cin>>option;
                   switch(option)
                    {
                      case 1:
                         cout<<"\n[[[% BALANCE INQUIRY %]]]\n";
                         cout<<"\n Your current balance is RS: "<< balance1<< endl;
                         continue;
                      case 2:
                         cout<<"\n[[[% WITHDRAW %]]]\n";
                         cout<<"Enter amount in RS: ";
                         cin>>withdraw;
                         balance1 = balance1 - withdraw;
                         cout<<"You withdrew RS: "<< withdraw<< endl;
                         cout<<"Your remaining balance is RS: "<< balance1<< endl;
                         continue;
                      case 3:
                          cout<<"\n[[[% DEPOSIT %]]]\n";
                          cout<<"Enter amount RS: ";
                          cin>>deposit;
                          balance1 = balance1 + deposit;
                          cout<<"You deposited RS: "<< deposit<< endl;
                          cout<<"Your new balance is RS: "<< balance1<< endl;
                          continue;
                      case 4:
                           cout<<"\n***[[[% EXIT MODE %]]]***\n";
                             break;
                      default:
                           cout<<"\n That is an invalid option Plz enter corrct option: \n";
                           continue; 
				  }
                break;
              }
         break;
       }
       if(i==2)
        {
           cout<<"\nCard is captured\n";
        }
       else
           cout<<"Pls try again!!!\n";
    }
 }
     else if(id == "YOGITA")
      {
         cout<<"\n WELCOME YOGITA \n";
         for (int i=0;i<3;i++)
          {
            cout <<"Please enter pin:\n";
            cin>>pin;
            double balance = 10000;
            balance1=balance;
            if (pin==8888)
             {
               for(int i=1;i<=10;i++)
                {
                  double withdraw, deposit;
                  int option;
                  cout<<"\n";
                  if(i==1)
                   { 
                      cout<<"*** Automated Teller Machine***"<< endl;
                      cout<<"Choose a Transaction:\n";
                      cout<<"\n";
                   }
                  cout<<" MAIN SCREEN \n";
                  cout<<"[1] Inquire Balance \n";
                  cout<<"[2] Withdraw \n";
                  cout<<"[3] Deposit \n";
                  cout<<"[4] Quit \n";
                  cout<<"\n";
                  cout<<"Enter Option:";
                  cin>>option;
                  switch(option)
                   {
                     case 1:
                        cout<<"\n[[[% BALANCE INQUIRY %]]]\n";
                        cout<<"\n Your current balance is "<< balance1<< endl;
                        continue;
                     case 2:
                        cout<<"\n[[[% WITHDRAW %]]]\n";
                        cout<<"Enter amount in RS: ";
                        cin>>withdraw;
                        balance1 = balance1 - withdraw;
                        cout<<"You withdrew RS: "<< withdraw<< endl;
                        cout<<"Your remaining balance is RS: "<< balance1<< endl;
                        continue;
                     case 3:
                        cout<<"\n[[[% DEPOSIT %]]]\n";
                        cout<<"Enter amount in RS: ";
                        cin>>deposit;
                        balance1 = balance1 + deposit;
                        cout<<"You deposited RS: "<< deposit<< endl;
                        cout<<"Your new balance is RS: "<< balance1<< endl;
                        continue;
                     case 4:
                        cout<<"\n***[[[EXIT MODE]]]***\n";
                        break;
                     default:
                        cout<<"\n That is an invalid option Plz enter correct option: \n";
                        continue;
                   }
                break;
              }
             break;
           }
       if(i==2)
         cout<<"\nCard is captured\n";
       else
          cout<<"Pls try again!!!\n";
      }
     }
     else
       cout<<"SOORY! YOUR ID IS INVALID"<<endl<<"Try With Correct ID";
   } 
   return 0;
 }
    void printstar(char ch , int n)
      {
        for(int i=1;i<=n;i++)
          {
            cout<< ch;
          }
        cout<<"\n";
     }
