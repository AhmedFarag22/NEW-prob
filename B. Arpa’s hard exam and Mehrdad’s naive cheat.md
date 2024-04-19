#include<bits/stdc++.h>
using namespace std;

void solve(){
   long long n;
   cin>>n;
    if(n == 0)
        cout<<1;
   else if(n % 4 == 0)
    cout<<6;
   else if(n %4 == 1)
    cout<<8;
   else if(n % 4 == 2)
    cout<<4;
   else if (n % 4 == 3){
		cout<<2;
	}

	/*
	1378(0) = 1              = 1
	1378(2) = 1911286        = 6
    1378(3) = 2633752108     =8
	*/

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();


}

