#include<bits/stdc++.h>
using namespace std;

 int n, m;
 int arr[11][11];
int ways(int num1) {
if(num1 >= m)
    return num1 == m;
return ways(num1+1) + ways(num1+2) + ways(num1+3);
}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);


cin>>n>>m;

cout<<ways(n);





}
