# jumpGame1
class Solution {
    public boolean canJump(int[] nums) {
        int n=nums.length;
        for(int i=0;i<nums.length;i++){
            if(nums[nums[i]]>n||(nums[i]+nums[i+nums[i]]>n)){
                return true;
            }
        }
        return false;
    }
}
