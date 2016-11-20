

###Problem
Paper streets are streets that are on a map, but do not exist in reality. A street can be planned but never built, and still end up on a map. Map makers also used to use paper streets to catch other companies copying and selling their maps.

Your challenge is to find the number of groups of paper streets on a map. A street is a line segment that starts and ends at intersections. A street is a paper street if it has no homes on it (a home on the end of the street doesn't count). A group is made of paper streets that all share at least one point with one other paper street in that group. 


      
###Counting Paper Streets Groups

![Map examples](map_examples.jpg)


###Inputs

The map is a grid of perpendicular lines. It's given to you as a list of X intercepts of vertical lines, then a list of Y intercepts of horizontal lines. The maps vary in size and are bound by the last lines given.

The homes are represented by X and Y coordinates. All numbers given are integers.

    x_intercepts = [0, 2, 4]
    y_intercepts = [0, 2]
    homes = [(0, 0), (0, 1), (0, 2), (1, 0), (1, 2), (2, 0), (2, 2), (3, 0), (3, 2), (4, 0), (4, 1), (4, 2)]

    2 X---X---X---X---X
      |       |       |
    1 X       |       X
      |       |       |
    0 X---X---X---X---X
      0   1   2   3   4

###Implementation
Modify the function `count_paper_streets` in solution.py to return the number of paper street groups.

###Tests
A test suite is included. Use `python -m unittest tests` to run it. Look to the test output for examples.

###Environment
Your code will be run on either Python 2.7.6 or 3.5.1 with Numpy installed. Our test runner tries Python 2 first, then 3 if there's a failure.

