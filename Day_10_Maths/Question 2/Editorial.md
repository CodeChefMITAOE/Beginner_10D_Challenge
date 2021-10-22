# Chocolate Frenzy Solution

Upon observation of few of the test cases, we can infer that initial number of chocolates will be N/C.  Then, after each step as long as wrappers are >m, chocolates will increment as the simple mathematical relation mentioned in the code below.

## Code :

		#define ll long long
		#include <bits/stdc++.h>
		using namespace std;

		int main()
		{
	    ll int t,N,C,M;
	    cin>>t;
		
		while(t--){
        cin>>N>>C>>M;
        
        ll int chocs = N/C;
        ll int wraps = chocs;
        
        while(wraps >= M){
        chocs += wraps/M;
        wraps = wraps/M + wraps%M;
        }
        
        cout<<chocs<<endl;
    }

    return 0;
	}
