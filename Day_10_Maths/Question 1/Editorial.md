  
# Fib-Reset Editorial

Type : Cake Walk

## Hints :

-  Just Iterate over the houses and check how many maximum coins of 5 thief can stole which can be easily calculated as 

```
total_valued_coin/5

Example :

N = 2
A[N] = 10,2

10/5 = 2
2/5 = 0

Answer = 2 + 0

```


## Code

    #include <iostream>
    using namespace std;
    
    int main() {
    	int n,ans = 0,house;
    	cin>>n;
    	for(int i=0;i<n;i++){
    	    cin>>house;
    	    ans += (house/5);
    	}
    	cout<<ans;
    	return 0;
    }

Link :  https://ide.geeksforgeeks.org/mzv0C6hu8C
