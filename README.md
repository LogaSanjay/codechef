#include<iostream>
#include<string.h>
using namespace std;
int main(){
string a,b;int i,l,j,flag=0,dec=1,t=0;
cin>>a;
for(i=0;i<100;)
{
  if(a[i]!=NULL) { i++;}
  else{break;}
}
l=i;
b=a;
for(i=0;i<l;i++)
{b[i]='0';}


while(dec){
for(j=l-1;j>=0;j--)
    {
        if(a[j]=='0')
        {
         flag=1;
        }
        else
        {
            l=j+1;
            break;
        }
        
    }
for(i=0;i<l;i++)
{
    if(a[i]=='0')
    {
        a[i]='1';
    }
    else
    {
        a[i]='0';
    }}if(a==b){dec=0;}
t++;
}cout<<t;return 0;}
