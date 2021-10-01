int Solution::solve(vector<int> &A, int B) {
    map<int, int> freq; 
    int cnt = 0;
    int xorr = 0; 
    for(auto it: A) {
        xorr = xorr ^ it; 

        if(xorr == B) cnt++; 

        if(freq.find(xorr ^ B) != freq.end()) 
            cnt += freq[xorr ^ B]; 
        
        freq[xorr] += 1; 
     }
     return cnt; 
}
