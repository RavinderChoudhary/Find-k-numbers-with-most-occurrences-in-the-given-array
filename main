#include <bits/stdc++.h>
using namespace std;

int main() {
	vector<int> arr = {7, 10, 11, 5, 2, 5, 5, 7, 11, 8, 9};
	int n = arr.size();
	int k = 4;
	
	unordered_map<int,int> mp;
	for(int i=0;i<n;i++)
	    mp[arr[i]]++;
	    
	vector<pair<int,int>> v;    
	for(auto it : mp)
	  v.push_back({it.first,it.second});
	  
	sort(v.begin(),v.end(),[](pair<int,int> p1,pair<int,int> p2) -> bool{
	   if(p1.second == p2.second)
	     return p1.first > p2.first;
	   return p1.second > p2.second;
	});
	
	int i=0;
	while(k > 0){
	    cout<<v[i].first<<" ";
	    i++;
	    k--;
	}
	return 0;
}

