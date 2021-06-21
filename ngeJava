class Solution {
    public int[] nextGreaterElements(int[] nums) {
        int n = nums.length; 
        int nge[] = new int[n];
        Stack<Integer> st = new Stack<>();
        for(int i = 2*n-1;i>=0;i--) {
            while(st.isEmpty() == false && st.peek() <= nums[i%n]) {
                st.pop(); 
            }
            
            if(i<n) {
                if(st.isEmpty() == false) nge[i] = st.peek(); 
                else nge[i] = -1; 
            }
            
            st.push(nums[i%n]);
        }
        return nge; 
    }
}
