#include<bits/stdc++.h>
using namespace std;

int gcd(int num1, int num2){

while(num2 != 0){
    return gcd(num2, num1%num2);
}
return num1;
}

int lcm(int num1, int num2){
return (num1*num2/gcd(num1, num2));
}

void solve(){

int num1, num2, num3, num4;
char c1, c2;
cin>>num1>>c1>>num2>>num3>>c2>>num4;
cout<<lcm(num1, num3)<<c1<<gcd(num2,num4);



}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();


}
