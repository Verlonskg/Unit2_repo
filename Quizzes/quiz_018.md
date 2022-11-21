
# Quiz_018

Lily was crossing a forest when she realizes that there is a tiger ahead of her who has seen Lily. 
Lily quickly takes out a matchbox from her bag and burns a matchstick, because the tiger is afraid of fire. 

A matchstick takes 5 seconds to burn completely.
The length of the forest that Lily needs to cross is l meters
Lily's speed is s cm/s

What is the minimum number of matchsticks Lily needs to burn to cross the forest safely.

```.py
def numberMatches(l:int, s:int) -> int:

    out = ""
    s1 = s/100
    l1 = (l/s1)/5
    m = l1%1
    if m > 0:
        l2 = 1-m
        l1 += l2
    out += f"{l1} matches"
    return out

out = numberMatches(l=100,s=100)
print(out)

out = numberMatches(l=250,s=110)
print(out)

out = numberMatches(l=500,s=150)
print(out)

out = numberMatches(l=12345,s=123)
print(out)
```
## Proof of work
![]()
**Fig. 1** Evidence that the program works for the four cases in the slide
