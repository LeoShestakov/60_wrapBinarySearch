# Wrap Binary Search 

0. y = log_2(x) means "2 raised to the power of y equals x".

1. The graph of y = log_2(x) has an asymptote of x = 0 and is constantly increasing, but the rate of increase decreases as x increases.

2. Recursive solution desc:
    0. Return the index of a given element of type Integer in an Ordered List using binary search.
    1. When asked to return the the index of a given element in an interval of an Ordered List, the recursive abstraction can
       return the index of the element in an interval of the Ordered List that is half the size.
    2. Decision: Is low > hi?
       
       If yes, return -2.
       
       If no, compare findMe to the element at index pageToCheck.
       
          If the comparison returns 0, return pageToCheck.
          
          If the comparison returns an int less than zero, return the index of the given element in the interval (low) to
          (pageToCheck - 1).
          
          If the comparison returns an int greater than zero, return the index of the given element in the interval 
          (pageToCheck + 1) to (hi).
