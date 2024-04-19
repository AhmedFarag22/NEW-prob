#include<bits/stdc++.h>
using namespace std;


void solve(){
int n;
cin>>n;
int arr[n], ma[1001]={0};

for(int i = 0; i < n; i++){
    cin>>arr[i];
    ma[arr[i]]++;
}
sort(ma, ma+1001, greater<int>());
int r = ma[0];


    if(n % 2 == 0){
        if(r <= (n/2))
            cout<<"YES";
        else
            cout<<"NO";
    }
    else{
        if(r <= (n/2+1))
            cout<<"YES";
        else
            cout<<"NO";

}

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();



}
