# CPP-Coding
BY Million Dollar Coder 

****************************************************************************
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

<img scr="https://www.google.com/url?sa=i&url=https%3A%2F%2Flo-victoria.com%2Fseries%2Fleetcode-challenge&psig=AOvVaw3jvzzfmFgnwp6g9aagJTid&ust=1707982289472000&source=images&cd=vfe&opi=89978449&ved=0CBMQjRxqFwoTCIimhP2nqoQDFQAAAAAdAAAAABAY" alt="not fount" width=250>
