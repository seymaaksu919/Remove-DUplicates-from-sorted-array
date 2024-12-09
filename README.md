# Remove-DUplicates-from-sorted-array
class Solution {
   
    public int removeDuplicates(int[] nums) {
        if(nums.length==0){
            return 0;
        }
       int k= 1;
        for(int i=1;i<nums.length;i++){
            if(nums[i]!=nums[i-1]){
                nums[k]=nums[i];
                k++;
            }
                

         }
            return k;
          
        }
        
    

public static void main(){
    Solution solution = new Solution();

   int [] nums= {1,1,2,2,3,4,5,5};
   int k= solution.removeDuplicates(nums);
        System.out.println("k değeri: " + k);

    for(int i=0; i<k; i++){
        System.out.println(nums[i]);

        }
        
       System.out.println("k değeri: " + k);

        
        }
}
