#include<bits/stdc++.h>
using namespace std;
/*
f(n) = -1+2-3+..n
*/

void solve(){
long long n;
cin>>n;

if(n % 2 == 0)
    cout<<n/2;
else
    cout<<n/-2-1;

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();



}
