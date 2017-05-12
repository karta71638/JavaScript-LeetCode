<h1>1.Two Sum</h1>

<h2>Description</h2>
<p>Given an array of integers, return <b>indices</b> of the two numbers such that they add up to a specific target.</p>
<p>You may assume that each input would have <b><i>exactly</i></b> one solution, and you may not use the <i>same</i> element twice.</p>
<p><b>Example:</b><br></p>

<pre>
Given nums = [2, 7, 11, 15], target = 9,
Because nums[<b>0</b>] + nums[<b>1</b>] = 2 + 7 = 9,
return [<b>0</b>, <b>1</b>].
</pre>

<h2>翻譯</h2>

<p>給一個裡面元素為int的陣列，陣列中會有兩個元素加起來等於target，回傳這兩個元素的位置。</p>
<p><b>範例：</b></p>
<p>[2, 7, 11, 15], target = 9，2+7=9，因此回傳[1,2]</p>

<h2>Solution</h2>

<pre><code>/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {

    for(var i = 0 ; i &lt; nums.length ; i++){
    
        var v = nums[i];

        for(var j = i+1 ; j &lt; nums.length ; j++ ){
            if(  nums[i] + nums[j]  == target ){
                return [i,j];
            }
        }

    }
};
</code></pre>
