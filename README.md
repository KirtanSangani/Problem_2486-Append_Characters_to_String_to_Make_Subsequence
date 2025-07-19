# Problem 2486: Append Characters To String To Make Subsequence

7/18/2025

## Thought Process
My initial thought process behind this problem was to just point at one of the strings and traverse through just one string. I later figured out that for this problem, that is not the case. 

##  Initial Solution
I initially tried to traverse through the string t, so that i can see how many letters were "found" by the end of traversing t. I would then return the difference between the len(t) and a count variable I created. I would quickly figure out that that is not the purpose of this problem. I was just looking at the similarities between the two strings and was not taking into account that I had to create a subsequence. 

Initial solution - N/A 

Complexity - O(len(t))

## Final Solution
I decided to use two pointers for both strings. This way, I would only move on in string t if I find a matching pair in string s. This way, I can find multiple characters that are the same in both strings in subsequence order also. I would create an i variable to traverse through string t and a j variable to traverse through string s and whenever I find that t[i] is equal to s[j], I would add 1 to i. Regardless of if the prior statement is true or false, I would add 1 to j. If either i or j are equal to their respective string's length, the while loop would end. I would then return the difference between len(t) and i, similarily to how I returned the difference between len(t) and count earlier. 

Final Solution - 48 ms

Complexity - O(n)

## Takeaways
I am starting to understand the usage of two pointers within a problem and am learning how to implement two pointers especially for traversing through multiple strings. With this method, I can also traverse through multiple Lists and dictionaries if necessary. 