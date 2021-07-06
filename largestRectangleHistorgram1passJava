class Solution {
    public int largestRectangleArea(int[] heights) {
        int n = heights.length; 
        Stack<Integer> st = new Stack<>();
        int maxA = 0; 
        for(int i = 0;i<=n;i++) {
            while(!st.isEmpty() && (i==n || heights[st.peek()] >= heights[i])) {
                int height = heights[st.pop()];
                int width; 
                if(st.isEmpty()) width = i; 
                else width = i - st.peek() - 1; 
                
                // cout << i << " " << width << " " << height << endl; 
                maxA = Math.max(maxA, width * height); 
            }
            st.push(i); 
        }
        return maxA;
    }
}
