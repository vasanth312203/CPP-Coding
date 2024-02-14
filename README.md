# CPP-Coding
BY Million Dollar Coder 

****************************************************************************


<img src="image4.jpg" alt="Not Found " width="2500" height="500">

<h1> Leet Code Problems </h1>

# 1768. Merge Strings Alternately

You are given two strings word1 and word2. Merge the strings by adding letters in alternating order, starting with word1. If a string is longer than the other, append the additional letters onto the end of the merged string.

Return the merged string.
# ANSWER :
```
class Solution {
public:
    string mergeAlternately(string word1, string word2) {
// BY Million Dollar Coder
         int i = 0,j=0; 
         string merged="";
    while( i < word1.length() && j<word2.length()){
      merged+=word1[i++];
      merged+=word2[j++];


}
while(i < word1.length()){
    merged+=word1[i++];
}
while( j<word2.length()){
    merged+=word2[j++];
}
    return merged;
 }
};
```


