#include<bits/stdc++.h>
using namespace std;

void solve(){
int n;
cin>>n;

map<string, int> foo;
for(int i = 0; i < n; i++){
    string key;
cin>>key;

if(foo[key] == 0)
    foo[key] = 1;
else
    foo[key]+=1;


}

map<string, int>::iterator my;
string resk = foo.begin()->first;
int resv = foo.begin()->second;
for(my = foo.begin(); my != foo.end(); my++){
    if(my->second > resv){
        resk = my->first;
        resv = my->second;
    }

}
cout<<resk;
}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();


}
