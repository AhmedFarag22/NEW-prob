#include<bits/stdc++.h>
using namespace std;



long long Knapsack(long long w, long long weight[], long long value[], long long item) {
if(w == 0 || item == 0)
    return 0;
if(weight[item-1] > w)
    return Knapsack(w, weight, value, item-1);
else {
    return max( value[item-1] + Knapsack(w-weight[item-1], weight, value, item-1),
            Knapsack(w, weight, value, item-1));
}

}

int main()
{
    std::ios_base::sync_with_stdio(0);
	cin.tie(NULL);

 long long n, w;
cin>>n>>w;
long long weight[n], value[n];

for(int i = 0; i<n; i++){
    cin>>weight[i]>>value[i];
}

cout<<Knapsack(w, weight, value, n);




}
