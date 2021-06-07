int isPossible(vector<int> &A, int pages, int students) {
    int cnt = 0;
    int sumAllocated = 0; 
    for(int i = 0;i<A.size();i++) {
        if(sumAllocated + A[i] > pages) {
            cnt++; 
            sumAllocated = A[i];
            if(sumAllocated > pages) return false; 
        }
        else {
            sumAllocated += A[i];
        }
    }
    if(cnt < students) return true; 
    return false; 
}
int Solution::books(vector<int> &A, int B) {
    if(B > A.size()) return -1; 
    int low = A[0]; 
    int high = 0;
    for(int i = 0;i<A.size();i++) {
        high = high + A[i]; 
        low = min(low, A[i]); 
    }
    int res = -1; 
    while(low <= high) {
        int mid = (low + high) >> 1; 
        //cout << low << " " << high << " " << mid << endl; 
        if(isPossible(A, mid, B)) {
            res = mid; 
            high = mid - 1; 
        }
        else {
            low = mid + 1; 
        }
    }
    // return res -> this is also correct
    return low; 
}
