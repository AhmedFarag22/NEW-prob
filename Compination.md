#include<bits/stdc++.h>
using namespace std;
//there are large number like !30

//nCr == nPr/!r

long long comp(long long n, long long r) {
    long long res = 1;
    long long temp = 2;
	for(int i = r+1; i<=n; i++){
        res*=i;
        if(temp <= n-r && res % temp == 0){
            res/=temp;
            temp++;
        }

	}
	return res;
}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);

 long long n, r;
cin>>n>>r;
if(r>n)
    cout<<0<<endl;
else
    cout<<comp(n,r);




}
