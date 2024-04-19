#include<bits/stdc++.h>
using namespace std;

void solve(){

   string s, ss;
   cin>>s;
   int ma = stoi(s);
   ss=s;
   s.erase(s.size()-1,1);
   ss.erase(ss.size()-2,1);

   cout<< max(max(stoi(s), stoi(ss)), ma);



}



int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();


}




