#include<iostream.h>
#include<stdio.h>
#include<conio.h>
#include<math.h>
#include<string.h>
void movie();
void mdate();
void mtime(int y);
void mticket();
void mseats(int z);
void mpayment(int p,char r[],int c[]);
void mgenticket(int q,float amo,char R[],int C[]);
void FC();
void contactus();
void rate();
char ch1[50],ch2[50],ch3[50],A[20],B[20],D[20];
int s,i,d,choice;
void main()
{
clrscr();
cout<<"\t\t\t\tWELCOME\n\n";
cout<<"\t\t*********SHOW TIME CINEMAS********\n";
cout<<"\t\t*      1.Book movie tickets       *\n";
cout<<"\t\t*      2.Food Court               *\n";
cout<<"\t\t*      3.CONTACT US               *\n";
cout<<"\t\t*      4.Rating                   *\n";
cout<<"Enter your Choice ";
cin>>choice;
switch(choice)
{
case 1:movie();break;
case 2:FC();break;
case 3:contactus();break;
case 4:rate();break;
default:cout<<"wrong option";
}
getch();
}
void movie()
{
clrscr();
cout<<"\n\t Movies\n\n";
cout<<"1.Anabelle Comes home(U/A)(English)\n\n";
cout<<"2.Kabir Singh(U/A)(Hindi)\n\n";
cout<<"3.Super 30(U/A)(Hindi)\n\n";
cout<<"Enter Choice ";
cin>>i;
while(i!=1 && i!=2 && i!=3)
{
cout<<"invalid Input.Try Again";
cin>>i;
}
if(i==1 || i==2 || i==3)
{
mdate();
}
}
void mdate()
{
clrscr();
int j;
cout<<"Enter date(1-31):";
cin>>j;
while((j>=1 && j<=31)!=1)
{
cout<<"Wrong Input.Try again.";
cin>>j;
}
d=j;
if(j>=1 && j<=31)
{
mtime(j);
}
}
void mtime(int y)
{
clrscr();
int k;
cout<<"Select Timings:";
if(y%2==0)
{
cout<<"1.10:00 a.m. \t 2.3:00 p.m. \t 3.8:00 p.m.\n\n";
cout<<"Enter Choice ";
cin>>k;
while(k!=1 && k!=2 && k!=3)
{
cout<<"Wrong Choice.Try again";
cin>>k;
}
s=k;
strcpy(A,"10:00 a.m.");
strcpy(B,"3:00 p.m.");
strcpy(D,"8:00 p.m.");
if(k==1 || k==2 || k==3)
{
mticket();
}
}
else
{
cout<<"1) 9:00 a.m.\t 2) 2:00 p.m.\t 3) 10:00 p.m.\n\n";
cout<<"Enter Choice ";
cin>>k;
while(k!=1 && k!=2 && k!=3)
{
cout<<"Wrong choice.Try again";
cin>>k;
}
s=k;
strcpy(A,"9:00 a.m.");
strcpy(B,"2:00 p.m.");
strcpy(D,"10:00 p.m.");
if(k==1 || k==2 || k==3)
{
mticket();
}
}
}
void mticket()
{
clrscr();
int m,t,l=0;char ch;
cout<<"Enter no.of tickets ";
cin>>m;
cout<<"\nDo you want more tickets?(y/n)";
cin>>ch;
if(ch=='y' || ch=='Y')
{
cout<<"Enter extra no. of tickets ";
cin>>l;
}
else if(ch=='n' || ch=='N')
{
cout<<"Proceed to seats section";
}
else
cout<<"Wrong input";
t=m+l;
cout<<"\nTotal tickets:"<<t;
mseats(t);
}
void mseats(int z)
{
int n,column[16];
char row[7];
cout<<"\n\n";
cout<<"\n                              SEAT ZONE \n\n";
cout<<"                    ALL EYES THIS WAY PLEASE\n\n";
cout<<"           A1 A2 A3 A4 A5 A6 A7 A8 | A9 A10 A11 A12 A13 A14 A15 A16\n";
cout<<"           B1 B2 B3 B4 B5 B6 B7 B8 | B9 B10 B11 B12 B13 B14 B15 B16\n";
cout<<"           C1 C2 C3 C4 C5 C6 C7 C8 | C9 C10 C11 C12 C13 C14 C15 C16\n";
cout<<"EXIT       D1 D2 D3 D4 D5 D6 D7 D8 | D9 D10 D11 D12 D13 D14 D15 D16         EXIT\n";
cout<<"           E1 E2 E3 E4 E5 E6 E7 E8 | E9 E10 E11 E12 E13 E14 E15 E16\n";
cout<<"           F1 F2 F3 F4 F5 F6 F7 F8 | F9 F10 F11 F12 F13 F14 F15 F16\n";
cout<<"           G1 G2 G3 G4 G5 G6 G7 G8 | G9 G10 G11 G12 G13 G14 G15 G16\n\n\n";
cout<<"                        EXIT               EXIT        ";
cout<<"\n\n Enter row and column:\n";
for(n=0;n<z;n++)
{
cout<<n+1<<".";
cin>>row[n]>>column[n];
}
mpayment(z,row,column);
}
void mpayment(int p,char r[],int c[])
{
float pay,gst=18.38;
cout<<"\n\n\n\t\t\tPAYMENT SECTION";
cout<<"\n\nCharges for per ticket:Rs 200";
pay=p*200;
cout<<"\nCharges for "<<p<<" tickets:Rs "<<pay;
cout<<"\n--------------------------";
cout<<"\ngst:Rs "<<gst;
pay=pay+gst;
cout<<"\n Total Charge:Rs "<<pay;
cout<<"\n---------------------------";
cout<<"\nPayable amount:Rs "<<ceil(pay);
mgenticket(p,pay,r,c);
}
void mgenticket(int q,float amo,char R[],int C[])
{
int g;
cout<<" \n\n\n\n   \t\t         SHOW TIME CINEMAS,NEW DELHI";
cout<<"\n\n\t\tMovie:";
strcpy(ch1,"Anabelle Comes Home(U/A)(English)");
strcpy(ch2,"Kabir Singh(U/A)(Hindi)");
strcpy(ch3,"Super 30(U/A)(Hindi)");
if(i==1)
cout<<ch1;
else if(i==2)
cout<<ch2;
else
cout<<ch3;
cout<<"\n\n\t\tDate:"<<d<<" July 2019";
cout<<"\n\t\tTime:";
switch(s)
{
case 1:cout<<A;break;
case 2:cout<<B;break;
case 3:cout<<D;break;
}
cout<<"\n\t\tAudi No.: 8";
cout<<"\n\t\tSeats:\n";
for(g=0;g<q;g++)
{
cout<<"\t\t"<<g+1<<"."<<R[g]<<C[g]<<endl;
}
cout<<"\n\t\tTotal charge: Rs "<<ceil(amo);
}
void FC()
{
clrscr();
cout<<"\t\t*Snacks*\t\t*Beverages*\t\t\n\n";
cout<<"\t1.french fries 150/- \t\t\t1.Cold Coffee 150/- \n\t2.Butter Popcorn 200/- \t\t\t2.Pepsi 70/- \n\t3.Chips 25/- \t\t\t\t3.Water 20/- ";
}
void contactus()
{
clrscr();
cout<<"\n\t\t\t SHOW TIME CINEMAS\n";
cout<<"\n\t\t213-Elen Street,New Delhi";
cout<<"\n\t\tTEL:0581-278134 FAX:45698879";
cout<<"\n\t\tEmail id: admin@stc.com";
}
void rate()
{
clrscr();
char u;
cout<<"Watched Movie(y/n)";
cin>>u;
if(u=='y')
{
cout<<"Rating allowed\n\n";
int w;
cout<<"Choose movie to rate:\n\n";
cout<<"1.Anabelle Comes home(U/A)(English)\n\n";
cout<<"2.Kabir Singh(U/A)(Hindi)\n\n";
cout<<"3.Super 30(U/A)(Hindi)\n\n";
cout<<"Enter Choice ";
cin>>w;
if(w==1)
{
int h;
cout<<"Movie\t\t\t\tRate(5)\n";
cout<<"Anabelle Comes home(U/A)(English)\t\t";
cin>>h;
while(h!=1 && h!=2 && h!=3 && h!=4 && h!=5)
{
if(h>5 || h<1)
{
cout<<"wrong rating.try again.";
cin>>h;
}
}
if(h==1 || h==2 || h==3 || h==4 || h!=5)
cout<<"Thank you for you feedback.Visit next time";
}
else if(w==2)
{
int h;
cout<<"Movie\t\t\t\tRate(5)\n";
cout<<"Kabir Singh(U/A)(Hindi)\t\t";
cin>>h;
while(h!=1 && h!=2 && h!=3 && h!=4 && h!=5)
{
if(h>5 || h<1)
{
cout<<"wrong rating.try again.";
cin>>h;
}
}
if(h==1 || h==2 || h==3 || h==4 || h!=5)
cout<<"Thank you for you feedback.Visit next time";
}
else if(w==3)
{
int h;
cout<<"Movie\t\t\t\tRate(5)\n";
cout<<"Super 30(U/A)(Hindi)\t\t";
cin>>h;
while(h!=1 && h!=2 && h!=3 && h!=4 && h!=5)
{
if(h>5 || h<1)
{
cout<<"wrong rating.try again.";
cin>>h;
}
}
if(h==1 || h==2 || h==3 || h==4 || h!=5)
cout<<"Thank you for you feedback.Visit next time";
}
else
cout<<"wrong input";
}
else if(u=='n')
cout<<"Rating not allowed";
else
cout<<"wrong input";
}






