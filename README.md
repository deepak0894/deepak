#include <bits/stdc++.h>
using namespace std;
void permute(string a,string b)
{  int k=0; 
    sort(a.begin(), a.end());
   do{ 
    int i=b.find(a); 
    if(i>=0){
    k++;
    }
   }
 while (next_permutation(a.begin(),a.end()));
 if(k>0)
 cout<<"True";
 else
 cout<<"False";
}
int main()
{
    string s,t;
    cin>>s>>t;
    permute(t,s);
    return 0;
}
