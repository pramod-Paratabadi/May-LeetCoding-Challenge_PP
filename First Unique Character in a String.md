## First Unique Character in a String

Given a string, find the first non-repeating character in it and return it's index. If it doesn't exist, return -1.

Examples:

s = "leetcode"
return 0.

s = "loveleetcode",
return 2.
Note: You may assume the string contain only lowercase letters.

## Answer

```python
class Solution:
    def firstUniqChar(self, s: str) -> int:
        li = collections.Counter(s)
        f=0
        # print(li)
        for i in s:
            if li[i]==1:
                f=1
                return s.index(i)
        if(f==0):
            return -1
        
        
```
