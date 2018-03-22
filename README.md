#include <bits/stdc++.h>

using namespace std;
int pos(int l)
{
   int x=l;
   return x;
}
int main()
{
    string s, t;
    while(cin>>s>>t)
    {
        int cnt=0,m;
        int j=0;
        bool x=false;
        for(int i=0; i<s.size(); i++)
       {
          for( j ;j<t.size(); j++)
         {
            if(s[i]==t[j])
            {
               cnt++;
               m=pos(j);
               break;
            }
         }
         j=m+1;
        }
    if(cnt==s.size())
        cout<<"Yes"<<endl;
    else
        cout<<"No"<<endl;
    }
    
    return 0;
}
