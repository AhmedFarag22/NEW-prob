#include<bits/stdc++.h>
using namespace std;

void solve(){
    vector<pair<int, int> >dr;
   int en, t;
   cin>>en>>t;
   for(int i = 0; i < t; i++){
        int k, p;
        cin>>k>>p;
        dr.push_back(make_pair(k,p));



   }


   sort(dr.begin(), dr.end());

   for(int i = 0; i < t; i++){
        if(en <= dr[i].first){
            cout<<"NO";
            return;
        }
        en+=dr[i].second;


   }
   cout<<"YES";

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();


}

