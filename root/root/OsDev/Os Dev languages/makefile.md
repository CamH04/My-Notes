# makefile
1.  `params = -m32`
2.  `%.o: %.cpp`
3.      `g++($params) -o $@ -c $<`

Line 2 Means:

in order to  create the object files from the cpp files do whats below

Line 3 Means:

use g++ with these parameters to compile

the ouptput (-o) should be the target file ($@) and we want to compile (-c) the input file ($<)