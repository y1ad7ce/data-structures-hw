HOMEWORK 1: MORPHOLOGICAL IMAGE PROCESSING

References:

https://stackoverflow.com/questions/7352099/stdstring-to-char
https://stackoverflow.com/questions/2797813/how-to-convert-a-command-line-argument-to-int
http://www.cplusplus.com/reference/sstream/istringstream/
https://www.learncpp.com/cpp-tutorial/713-command-line-arguments/
http://www.cplusplus.com/reference/string/string/getline/
https://stackoverflow.com/questions/9597963/why-does-stdgetlinecin-number-give-a-no-matching-function-for-call-error
https://stackoverflow.com/questions/13571565/c-copying-multidimensional-vector
https://stackoverflow.com/questions/25026958/what-is-the-best-way-to-copy-a-2d-vector

Test case 1:
XXX........X..
X.X.......XXXX
X.X.......XXX.
.X..XXX.......
....X.X...X.XX
X...X.X..X...X
X...XXX..X...X
.........XXXX.

Results:

Dilation:
XXXX......XXXX
XXXX.....XXXXX
XXXXXXX..XXXXX
XXXXXXXX..XXXX
XX.XXXXX.XXXXX
XX.XXXXXXXX.XX
XX.XXXXXXXXXXX
X...XXX.XXXXXX

Erosion:
X.............
...........X..
..............
..............
..............
..............
..............
..............

Opening:
XX.........X..
X.........XXX.
...........X..
..............
..............
..............
..............
..............

Closing:
XXX........XXX
XXX.......XXXX
XXXX......XXXX
XX.XXXX....XXX
X...XXX...X.XX
X...XXXX.X...X
X...XXX.XXX.XX
.....X...XXXXX

Test case 2:
X...................XXXXX...........X.
......XXXXX..........X..............XX
......XX..XXX.........XXX.............
......XX....XX........................
......XX.X...X....X...................
......XX....X.....X.X.....XXXXX.......
......XXXXXXXXX...X.X.....XXXXX.......
.......XXXXXXXX.....X.....X.XXX.......
........XXX...X...........X.XXX.......
........XXX...X...XXX.....X.XXX.......
....XX..XXX...X...........X.XXX.......
.....X..XXXXXXX....XXX....X.XXX.......
.....X..XXXXXXX...............XXX.....
...XXX..XXXXXXXXX......XXX............
X........XXX...XX.....XX............X.
XX..........XXXXX...XXXXX.............

Results:

Dilation: 
XX....XXXXX........XXXXXXX.........XXX
X....XXXXXXXX.......XXXXX..........XXX
.....XXXXXXXXX.......XXXXX..........XX
.....XXXXXXXXXX...X...XXX.............
.....XXXXXX.XXX..XXXX.....XXXXX.......
.....XXXXXXXXXX..XXXXX...XXXXXXX......
.....XXXXXXXXXXX.XXXXX...XXXXXXX......
......XXXXXXXXXX..XXXX...XXXXXXX......
.......XXXXXXXXX..XXX....XXXXXXX......
....XX.XXXXX.XXX.XXXXX...XXXXXXX......
...XXXXXXXXXXXXX..XXXX...XXXXXXX......
....XXXXXXXXXXXX..XXXXX..XXXXXXXX.....
...XXXXXXXXXXXXXX..XXX.XXXX.XXXXXX....
X.XXXXXXXXXXXXXXXX....XXXXX...XXX...X.
XX.XXX..XXXXXXXXXX..XXXXXX.........XXX
XXX......XXXXXXXXX.XXXXXXX..........X.

Erosion:
.....................X................
......................................
......................................
......................................
......................................
......................................
.......X....X...............XX........
........XXX..................X........
.........X...................X........
.........X...................X........
.........X...................X........
.........XX...........................
.........XXXXX........................
.........XXX..........................
......................................
X..............X......XX..............

Opening:
....................XXX...............
.....................X................
......................................
......................................
......................................
.......X....X...............XX........
......XXXXXXXX.............XXXX.......
.......XXXXXX...............XXX.......
........XXX.................XXX.......
........XXX.................XXX.......
........XXX.................XXX.......
........XXXXXX...............X........
........XXXXXXX.......................
........XXXXXX........................
X........XXX...X......XX..............
XX............XXX....XXXX.............

Closing:
X......XXX..........XXXXX...........XX
......XXXXX..........XXX............XX
......XXXXXXX.........XXX.............
......XXXXX.XX........................
......XXXX...X....X...................
......XXXXX.XX....XXX.....XXXXX.......
......XXXXXXXXX...XXX.....XXXXX.......
.......XXXXXXXX....XX.....XXXXX.......
........XXXX.XX....X......XXXXX.......
........XXX...X...XXX.....XXXXX.......
....XX.XXXXX.XX....XX.....XXXXX.......
.....XXXXXXXXXX....XXX....X.XXXX......
....XXXXXXXXXXXX.........X....XXX.....
...XXX..XXXXXXXXX......XXX............
X........XXXXXXXX.....XXX...........X.
XX........XXXXXXX...XXXXX.............
