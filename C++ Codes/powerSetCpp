vector<string> AllPossibleStrings(string s){
		    int n = s.size(); 
		    vector<string> ans; 
		    for(int num = 0; num < (1 << n); num++) {
		        string sub = ""; 
		        for(int i = 0;i<n;i++) {
		            if(num & (1<<i)) {
		                sub += s[i];
		            }
		        }
		        if(sub.size() > 0)
		            ans.push_back(sub);
		    }
		    sort(ans.begin(), ans.end()); 
		    return ans; 
		}
