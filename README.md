# CodingPractice
Basic Coding Practice By Gurpreet
## Problems

```
1. Write a program that manipulates a given string s by k characters.[Last values should wrap up in a circular
fashion and length of the manipulated string remains same]
Guru,k=1 > uGur
```
## Code 1
```
def shift_by_k(s,k):
  shifted_s=[0 for i in range(len(s))]
  for i in range(len(s)):
    shifted_s[(i+k)%len(s)]=s[i]
  return shifted_s
  
```
