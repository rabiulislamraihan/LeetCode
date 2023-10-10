#include<bits/stdc++.h>
using namespace std;

/*
Given an integer array nums,
return true if any value appears at least twice in the array,
and return false if every element is distinct.
                                            */

// O(n^2), O(1)
class Solution1 {
public:
    bool containsDuplicate(vector<int>& nums) {
        for (int i = 0; i < nums.size() - 1; i ++) {
            for (int j = i + 1; j < nums.size(); j ++) {
                if(nums[i] == nums[j]) {
                    return true;
                }
            }
        }
        return false;
    }
};

// O(n*log(n)), O(1)
class Solution2 {
public:
    bool containsDuplicate(vector<int>& nums) {
        sort(nums.begin(), nums.end());
        for (int i = 0; i < nums.size() - 1; i ++) {
            if (nums[i] == nums[i + 1]) {
                return true;
            }
        }
        return false;
    }
};

// O(n), O(n)
class Solution3 {
public:
    bool containsDuplicate(vector<int>& nums) {
        unordered_set <int> st;
        for (int i = 0; i < nums.size(); i ++) {
            if(st.count(nums[i])) {
                return true;
            }
            st.insert(nums[i]);
        }
        return false;
    }
};


int32_t main() { 
    ios_base::sync_with_stdio(false), cin.tie(NULL), cout.tie(NULL);

}
