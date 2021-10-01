class Solution {
public:
    int lengthOfLongestSubstring(string s) {
        int left = 0, right = 0; 
        set<char> st; 
        int n = s.size();
        int len = 0;
        while(right < n) {
            if(st.find(s[right]) != st.end()) {
                st.erase(s[left]);
                left++;
            } else {
                st.insert(s[right]); 
                len = max(len, right - left + 1); 
                right++; 
            }
        }
        return len; 
    }
};
