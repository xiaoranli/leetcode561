# 2、leetcode561. 数组拆分 I
解法一：
--  
思路：
--
    排序即可。  
代码： 
--
<pre>
/**
 * @author lihe
 * @date 2019/10/22 12:52
 * @descriptor  561. 数组拆分 I
 */
public class ArrayPairSum_561 {
    public static int arrayPairSum(int[] nums) {
        Arrays.sort(nums);
        int count = 0;
        for(int i = 0;i < nums.length;i++){
            if(i % 2 == 0)
                count += nums[i];
        }
        return count;
    }
    public static void main(String[] args) {
        int[] arr = {1,4,3,2};
        int i = arrayPairSum(arr);
        System.out.println(i);
    }
}
</pre>
