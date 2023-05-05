Test purpose:

See whether the example in the program description produces the output it says it should

Text input:

!@£$%^&*!@£$%^&*

Wrap limit:

7

Expected output:

!@£$%^&
*!@£$%^
&*

Actual output:
zsh: event not found: @£
--END OF FILE--
_______________________________________

Test purpose:

See whether the example in the program description produces the output it says it should

Text input:

12345678901234567890123

Wrap limit:

10

Expected output:

1234567890
1234567890
123

Actual output:
1234567890
1234567890
123
END OF FILE
--END OF FILE--
_______________________________________

Test purpose:

See how the program behaves when given a word that
is longer than the wrap limit

Text input:

This is a long word: incomprehensibility

Wrap limit:

16

Expected output:

This is a long 
word: incomprehe
nsibility

Actual output:
Traceback (most recent call last):
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 38, in <module>
    for sieqngpr in dfuydirw(sys.argv[2], int(sys.argv[1]), []):
                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 23, in dfuydirw
    return dfuydirw(pwuvmeal[fneovhye+1:], pwndysaq, jeodnshc)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 23, in dfuydirw
    return dfuydirw(pwuvmeal[fneovhye+1:], pwndysaq, jeodnshc)
           ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 21, in dfuydirw
    fneovhye = pwuvmeal[:pwndysaq-1].rindex(" ")
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
ValueError: substring not found
--END OF FILE--
_______________________________________

Test purpose:

See how the program behaves when given a very short
wrap limit

Text input:

snap crackle pop

Wrap limit:

2

Expected output:

sn
ap
 c
ra
ck
le
 p
op

Actual output:
Traceback (most recent call last):
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 38, in <module>
    for sieqngpr in dfuydirw(sys.argv[2], int(sys.argv[1]), []):
                    ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 21, in dfuydirw
    fneovhye = pwuvmeal[:pwndysaq-1].rindex(" ")
               ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
ValueError: substring not found
--END OF FILE--
_______________________________________

Test purpose:

See whether the example in the program description produces the output it says it should

Text input:

The man in black fled across the desert, and the gunslinger followed

Wrap limit:

26

Expected output:

The man in black fled 
across the desert, and the
gunslinger followed
--END OF FILE--

Actual output:
The man in black fled
across the desert, and the
 gunslinger followed
END OF FILE
_______________________________________

Test purpose:

See if a letter can be accepted as a wrap limit

Text input:

The man in black fled across the desert, and the gunslinger followed

Wrap limit:

f

Expected output:

Error message

Actual output:
Traceback (most recent call last):
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 38, in <module>
    for sieqngpr in dfuydirw(sys.argv[2], int(sys.argv[1]), []):
                                          ^^^^^^^^^^^^^^^^
ValueError: invalid literal for int() with base 10: 'f'
_______________________________________

Test purpose:

See if punctuation is accepted as a wrap limit

Text input:

The man in black fled across the desert, and the gunslinger followed

Wrap limit:

&

Expected output:

Error message

Actual output:
[1] 4901
zsh: command not found: The man in black fled across the desert, and the gunslinger followed
Traceback (most recent call last):                                              
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 38, in <module>
    for sieqngpr in dfuydirw(sys.argv[2], int(sys.argv[1]), []):
                             ~~~~~~~~^^^
IndexError: list index out of range
[1]  + 4901 exit 1     python3 wrap_it.py
_______________________________________

Test purpose:

Demonstrate what happens when no wrap limit is given

Text input:

The man in black fled across the desert, and the gunslinger followed

Wrap limit:

*blank*

Expected output:

Error message

Actual output:
Traceback (most recent call last):
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 38, in <module>
    for sieqngpr in dfuydirw(sys.argv[2], int(sys.argv[1]), []):
                             ~~~~~~~~^^^
IndexError: list index out of range
_______________________________________

Test purpose:

Demonstrate what happens if no input is given

Text input:

*blank*

Wrap limit:

*blank*

Expected output:

Error message

Actual output:
Traceback (most recent call last):
  File "/Users/samgeorge/MayProjects/TestingIntro/intro-to-testing/phase2/05_resources/wrap_it.py", line 38, in <module>
    for sieqngpr in dfuydirw(sys.argv[2], int(sys.argv[1]), []):
                             ~~~~~~~~^^^
IndexError: list index out of range
_______________________________________