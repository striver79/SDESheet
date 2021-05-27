int singleNonDuplicate(vector<int>& nums) {
        int low = 0, high = nums.size() - 2; 
        while(low <= high) {
            int mid = (low + high) >> 1; 
            if(nums[mid] == nums[mid^1]) {
                low = mid + 1; 
            } 
            else {
                high = mid - 1; 
            }
        }
        return nums[low]; 
    }
