class Solution {
    public int[] shuffle(int[] nums, int n) {
        int x=0;
        int y=n;//3
        int arr[]=new int[nums.length];
        for(int i=0;i<nums.length;i++)//[2,3,5,4,1,7] 
        {
            if(i%2==0)//
            {
                arr[i]=nums[x];//2
                x++;//1

            }
            else
            {
               arr[i]=nums[y];//3
               y++;//4
            }

        }
        return arr;
    }
}
