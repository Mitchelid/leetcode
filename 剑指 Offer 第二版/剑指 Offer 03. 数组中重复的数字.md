![image-20220102212235707](..\image\image-20220102212235707.png)

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

