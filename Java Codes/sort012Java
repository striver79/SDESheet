class Solution {
    public void sortColors(int[] nums) {
        int lo = 0; 
        int hi = nums.length - 1; 
        int mid = 0; 
        int temp; 
        while (mid <= hi) { 
            switch (nums[mid]) { 
                case 0: { 
                    temp = nums[lo]; 
                    nums[lo] = nums[mid]; 
                    nums[mid] = temp; 
                    lo++; 
                    mid++; 
                    break; 
                } 
                case 1: 
                    mid++; 
                    break; 
                case 2: { 
                    temp = nums[mid]; 
                    nums[mid] = nums[hi]; 
                    nums[hi] = temp; 
                    hi--; 
                    break; 
                } 
            } 
        }
    }
}
