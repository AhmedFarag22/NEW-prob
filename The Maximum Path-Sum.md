#include<bits/stdc++.h>
using namespace std;

 int n, m;
 int arr[11][11];
int path(int st, int en) {

if(st == n-1 && en == m-1)
    return arr[st][en];
else if(st == n+1 || en == m+1)
    return -1000000;
int right = path(st, en+1);
int down = path(st+1, en);


return arr[st][en]+max(right, down);
}
/*
3 3
5 2 4
1 3 5
9 2 7


24
*/
int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);


cin>>n>>m;
  arr[n][m];
for(int i = 0; i<n; i++){
    for(int j = 0; j<m; j++){
        cin>>arr[i][j];
}

}
cout<<path(0,0);





}
