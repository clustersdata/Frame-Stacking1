# Frame-Stacking1

Frame Stacking

Description
Consider the following 5 picture frames placed on an 9 x 8 array.


........ ........ ........ ........ .CCC....

EEEEEE.. ........ ........ ..BBBB.. .C.C....

E....E.. DDDDDD.. ........ ..B..B.. .C.C....

E....E.. D....D.. ........ ..B..B.. .CCC....

E....E.. D....D.. ....AAAA ..B..B.. ........

E....E.. D....D.. ....A..A ..BBBB.. ........

E....E.. DDDDDD.. ....A..A ........ ........

E....E.. ........ ....AAAA ........ ........

EEEEEE.. ........ ........ ........ ........

    1        2        3        4        5   


Now place them on top of one another starting with 1 at the bottom and ending up with 5 on top. If any part of a frame covers another it hides that part of the frame below.

Viewing the stack of 5 frames we see the following.


.CCC....

ECBCBB..

DCBCDB..

DCCC.B..

D.B.ABAA

D.BBBB.A

DDDDAD.A

E...AAAA

EEEEEE..






In what order are the frames stacked from bottom to top? The answer is EDABC.

Your problem is to determine the order in which the frames are stacked from bottom to top given a picture of the stacked frames. Here are the rules:

1. The width of the frame is always exactly 1 character and the sides are never shorter than 3 characters.

2. It is possible to see at least one part of each of the four sides of a frame. A corner shows two sides.

3. The frames will be lettered with capital letters, and no two frames will be assigned the same letter.

Input

Each input block contains the height, h (h<=30) on the first line and the width w (w<=30) on the second. A picture of the stacked frames is then given as h strings with w characters each.
Your input may contain multiple blocks of the format described above, without any blank lines in between. All blocks in the input must be processed sequentially.

Output

Write the solution to the standard output. Give the letters of the frames in the order they were stacked from bottom to top. If there are multiple possibilities for an ordering, list all such possibilities in alphabetical order, each one on a separate line. There will always be at least one legal ordering for each input block. List the output for all blocks in the input sequentially, without any blank lines (not even between blocks).

Sample Input

9
8
.CCC....
ECBCBB..
DCBCDB..
DCCC.B..
D.B.ABAA
D.BBBB.A
DDDDAD.A
E...AAAA
EEEEEE..

Sample Output

EDABC
