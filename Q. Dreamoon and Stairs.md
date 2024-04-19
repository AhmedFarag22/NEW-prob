#include<bits/stdc++.h>
using namespace std;



void solve(){
int n, m, mid;
cin>>n>>m;
if(n % 2 == 0)
     mid = n/2;
else
     mid = n/2+1;

    for(int i = mid; i <= n; i++){
        if(i % m == 0){
            cout<<i;
            return;

        }
    }
cout<<-1;
}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();



}
