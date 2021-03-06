## EA Programming Excercises by Don Munro:

All solutions assume user will be using a Python 2.7+ capable environment.  The solutions
can be cloned using the following command:
```
cd $YOUR_WORK_DIR
git clone https://github.com/don-munro/problems
```

Or alternatively the changes can be viewed/used as a pull request as per instructions
from Travis.

Sample input/output are as follows:

### Common Subsequence

```
cd $YOUR_WORK_DIR/problems/don_munro
python common_subsequence.py ./subsequence.in
LCS for XMJYAUZ and MZJAWXU : MJAU
LCS for abcdef and acbef : abef
```

### Common Substring

```
cd $YOUR_WORK_DIR/problems/don_munro
python common_substring.py 'Everything is awesome!' 'Hello World is awesome!'
 is awesome!
```

Solution on hand uses a simplified version of the Common Subsequence solution.
It treats the input parameter as strings and does not take a word-by-word approach.
'''
python common_substring.py 'Everything is awesome!' 'He stared in awe!'
 awe
'''
Note that the match includes the whitespace - ' awe'

### Fibonacci Sequence
```
cd $YOUR_WORK_DIR/problems/don_munro
python fibonacci.py 8
0, 1, 1, 2, 3, 5, 8, 13
```

Limitations:
 - As it stands there is no limit on the size of a sequence that can be requested.
   While Python seems to handle precision of large values, there is an issue with
   max recurrsion depth being reached.  This is left as a know vulnerability at this
   time.

### Essay Monkey

The essay Monkey should be considered a work in progress at this time with apologies
(but no excuse) as timelines and previous commitments make it look like this may
not be completed before the interview tomorrow AM.  There are 3 other solutions here
but I thought I'd try this one as well given the substring and subsequence problems are
similar.