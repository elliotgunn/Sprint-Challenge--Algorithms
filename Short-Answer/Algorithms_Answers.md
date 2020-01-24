#### Please add your answers to the ***Analysis of  Algorithms*** exercises here.

## Exercise I

a) O(n) as steps increases with value of n


b) O(nlog(n)) as there is a nested loop for n but...


c) O(n) as the function is recursively called n times before reaching base case

## Exercise II

# need to find the floor that is resulting in broken eggs
Option 1:

dropped = 0
floor = range(n)
EggsBroken = False

for f in range(n):
    if EggsBroken != True:
        dropped += 1
    else:
       return f
       break

runtime complexity:
O(n) as steps increase with value of n

Option 2: Use something similar to binary search since the floors are like a sorted list

def find_floor(n):
    base case: when down to two floors. if not one floor then it's the other. 

    eggs_broken = 0
    find midpoint, split into two sub-lists
        lower =
        upper =
        if midpoint breaks, try lower half:
            eggs_broken += 1
            # recursion
            find_floor(range(lower))
        else, try upper half:
            find_floor(range(upper))

runtime complexity: O(log n) as eliminate half possible entries each round (log base 2)






