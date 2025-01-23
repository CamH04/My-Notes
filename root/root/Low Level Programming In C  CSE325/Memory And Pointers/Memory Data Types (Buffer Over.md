# Memory Data Types (Buffer Overflow EG)
Type Overflow Example
---------------------

Reference

8bits = Char

16bits = short

32bits = int

`short number = 32767 + 1;`

`printf("%d \n", number);`

This causes a buffer overflow as 32767 is the largest value you can represent in a short and you add 1.

that the causes the sign bit to be flipped as 1 and the rest become 0 because of binary addition, creating the smallest possible value of 

\-32768