#include<bits/stdc++.h>
using namespace std;
/*
inputs
3 3 5
1 2 3
4 5 6
7 8 9
g 3 2
r 3 2
c 2 3
g 2 2
g 3 2


outputs
8
9
6
*/

void solve2(){
int n, m, k;
cin>>n>>m>>k;

int arr[1+n][1+m];

for(int i = 0; i <= n; i++){
   for(int j = 0; j <= m; j++){
    cin>>arr[i][j];
    }
}
for(int i = 0; i < k; i++){
    char c;
    int x , y ;
    cin>>c>>x>>y;
x--;y--;
        for(int j = 0; j < m; j++){
            swap(arr[x][j], arr[y][j]);
        }

}

for(int i = 0; i < n; i++){
   for(int j = 0; j < m; j++){
    cout<<arr[i][j];
    }
    cout<<endl;
}
}
void solve(){

int n, m, k;
cin>>n>>m>>k;

int arr[n+1][m+1] = {0}, R[1+n] = {0}, C[1+m] = {0};

for(int i = 1; i <= n; i++){
   for(int j = 1; j <= m; j++){
    cin>>arr[i][j];
    C[j] = j;
    }
    R[i] = i;
}

for(int i = 0; i < k; i++){
    char c;
    int x, y;
    cin>>c>>x>>y;

    if(c == 'r'){


            swap(R[x], R[y]);

    }
    if(c == 'c'){

            swap(C[x], C[y]);

    }
    if(c == 'g')
        cout<<arr[R[x]][C[y]]<<endl;;
}

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);
    solve();



}
