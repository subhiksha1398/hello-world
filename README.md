# hello-world
# Line clipping Algorithm using Nicholl–Lee–Nicholl algorithm.
NLN- is another algorithm in Line clipping which has 3 possible positions for Line endpoint P1 such as :
1. in window region 2. in edge region  3. in corner region. 
According to where the point lies we need to find out the intersection and  then draw a vertex where point lies, so that we we can find intersection points.
Name the intersection point for reference and check intersection pointslies between the points p1 &p2 also check which region it falls that  is [LRBT] Left,Right,Bottom,Top.
Areas are then designated as L, LT, LB, or TR, depending on the location of the initial point. 
Then the other end point of the line is checked against these areas.
If a line starts in the L area and finishes in the LT area then the algorithm concludes that the line should be clipped at xw (max). 
Thus the number of clipping points is reduced to one, compared to other algorithms that may require two or more clipping.
Possible cases are there:
CASE1: In inside case, the areas are named T for top, L for left, R for right, and B for bottom.
CASE2: In left case, the areas are named L for left, TL for top and left, LR for left and right, and TB for top and bottom.
CASE3:In top-left case, the areas are named L for left , T for top, TR for top and right, LB for left and bottom, and TB for top and bottom or LR for left and right.
The last step is just locate the end point of the line that wants to be clipped, and clipped it according to the name of that area against the side(s) of the clipping window.
