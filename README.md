# CPP-Coding
BY Million Dollar Coder 

****************************************************************************


<img src="image4.jpg" alt="Not Found " >

<h1> Leet Code Problems </h1>

# 1768. Merge Strings Alternately

# QUESTION :

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

<img src="image.jpg" alt="Not Found " >

*************************************************************

# 1431. Kids With the Greatest Number of Candies

# QUESTION :
There are n kids with candies. You are given an integer array candies, where each candies[i] represents the number of candies the ith kid has, and an integer extraCandies, denoting the number of extra candies that you have.

Return a boolean array result of length n, where result[i] is true if, after giving the ith kid all the extraCandies, they will have the greatest number of candies among all the kids, or false otherwise.

Note that multiple kids can have the greatest number of candies.

# ANSWER :

```
class Solution {
public:
    vector<bool> kidsWithCandies(vector<int>& candies, int extraCandies) {

        vector<bool> result;
        int size = candies.size();

        // int maxvalue = candies[0];
        // for (int j = 0; j < size; j++) {
        //     maxvalue = max(maxvalue, candies[j]);
        // }

        int maxvalue = *max_element(candies.begin(), candies.end());

        for (int i = 0; i < size; i++) {
            if (candies[i] + extraCandies < maxvalue) {
                result.push_back(false);

            } else {
                result.push_back(true);
            }
        }
        return result;
    }
};

```

<img src="image.jpg" alt="Not Found " >

*************************************************************
