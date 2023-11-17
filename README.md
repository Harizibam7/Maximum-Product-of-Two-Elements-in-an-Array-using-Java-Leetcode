# Maximum-Product-of-Two-Elements-in-an-Array-using-Java-Leetcode


    class Solution {
        public int maxProduct(int[] nums) {
            int result = 0;
            int mul =0;
            for(int i =0; i<nums.length-1;i++){
                for(int j =i+1;j<nums.length;j++){
                    mul = (nums[i]-1)*(nums[j]-1);
                        if(mul > result){
                        result = mul;
                    }
                }
                
            }
            return result;
        }
    }
