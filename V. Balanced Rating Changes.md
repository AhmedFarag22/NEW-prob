#include<bits/stdc++.h>
using namespace std;

// ceil(-0.5) = -0
// double r = (double)x/2;
void solve(){
int n;
cin>>n;

bool b = 0;
for(int i = 0; i < n; i++){
    int x;
    cin>>x;
    double r = (double)x/2;

    if(x%2 == 0)
        cout<<x/2<<endl;
    else{
        if(!b){
            if(r == -0.5)
                cout<<0<<endl;
            else
                cout<<ceil(r)<<endl;
            b = 1;
        }
        else{

                cout<<floor(r)<<endl;
            b = 0;
        }
    }
}

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();
    cout<< ceil(-0.5); // = -0


}
