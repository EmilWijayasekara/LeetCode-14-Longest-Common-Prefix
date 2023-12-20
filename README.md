
# LeetCode Practice  (Day 4)
## Achievements
[![Leetcode-copy.jpg](https://i.postimg.cc/WzrtR30J/Leetcode-copy.jpg)](https://postimg.cc/5Q4fLf7x)

## About the problem
- *Problem Number* : 14
- *Problem Name* :  [Longest Common Prefix](https://leetcode.com/problems/longest-common-prefix/)
- *Problem difficulty* : Easy (41.91%) 🟢
- *Category* : Algorithms
- *Programming language used* - Java

## Problem


Write a function to find the longest common prefix string amongst an array of strings.
If there is no common prefix, return an empty string  `""`.

**Example 1:**

```
Input: strs = ["flower","flow","flight"]
Output: "fl"
```

**Example 2:**

```
Input: strs = ["dog","racecar","car"]
Output: ""
Explanation: There is no common prefix among the input strings.
```

**Constraints:**

-   `1 <= strs.length <= 200`
-   `0 <= strs[i].length <= 200`
-   `strs[i]`  consists of only lowercase English letters.

## Approach Explanation
First, filter out the empty String arrays and return `""`.
Then I sorted the array, and from this I can get the alphabetical order of the string array. for example 

```
example 1
original String  = ["flower", "flow", "flight"]
after the sort = ["flight", "flow", "flower"]

example 2
original String  = ["Emil", "Ashi", "Thimira"]
after the sort = ["Ashi","Emil","Thimira"]
```

From this, I can compare just the first word and last word in the string. Because the words in between are always sorted accordingly. Then just using a while loop I compared the first and last word in the string array. Then just using a while loop I compared the first and last word in the string array. If both words have the same letters then increment the counter variable, otherwise we break from the loop. If the counter variable value is equal to zero that means there is no common prefix in these strings, then we must return `""`. If the counter value is greater than zero, then using `substring()` method we return common prefix 

### If you have suggestions for improvement or would like to contribute to this solution, feel free to create a pull request. 🙌😇
