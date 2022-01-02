![image-20220102212235707](https://github.com/Mitchelid/leetcode/blob/main/%E5%89%91%E6%8C%87%20Offer%20%E7%AC%AC%E4%BA%8C%E7%89%88/image/image-20220102212235707.png)

#### 方法一 unordered_map

```c++
class Solution {
public:
    int findRepeatNumber(vector<int>& nums) {
        unordered_map<int,int> um;
        for(auto a : nums){
            if(um[a])
                return a;
            um[a] = 1;
        }
        return 0;
    }
};
```

