public class Solution {
    private int countSmallerThanMid(ArrayList<Integer> row, int mid) {
        int l = 0, h = row.size() - 1; 
        while(l <= h) {
            int md = (l + h) >> 1; 
            if(row.get(md) <= mid) {
                l = md + 1;
            }
            else {
                h = md - 1;
            }
        }
        return l; 
    }
    public int findMedian(ArrayList<ArrayList<Integer>> A) {
        int low = Integer.MIN_VALUE;
        int high = Integer.MAX_VALUE; 
        int n = A.size();
        int m = A.get(0).size(); 
        while(low <= high) {
            int mid = (low + high) >> 1; 
            int cnt = 0;
            for(int i = 0;i<n;i++) {
                cnt += countSmallerThanMid(A.get(i), mid); 
            }
    
            if(cnt <= (n * m) / 2) low = mid + 1; 
            else high = mid - 1; 
        }
        return low; 
    }
}
