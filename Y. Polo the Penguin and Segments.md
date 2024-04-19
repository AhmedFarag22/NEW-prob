#include<bits/stdc++.h>
using namespace std;

void solve(){

int n,k;
cin>>n>>k;
int co = 0;
for(int i = 0; i < n; i++){
    int x,y;
    cin>>x>>y;
    co+=y-x+1;
}

co%=k;

if(co == 0)
    cout<<0;
else
    cout<<k-co;

}


int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();



}
