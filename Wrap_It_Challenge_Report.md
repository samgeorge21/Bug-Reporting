WRAP IT PROGRAM CHALLENGE REPORT

** Details of each test will be in the accompanying document: Wrap_It_Challenge_Outputs.md **

Test 1:
With this test I was aiming to see what would happen if a string only containing mixed punctuation was entered.
I had expected the output to wrap around the punctuation each time the limit was reached and then start a new line, although from earlier conversations I was aware that some punctuation could cause problems.
The actual outcome was that an error message was received, stating that the event had not been found.

Test 2:
The aim of this test was similar to the previous one, but looked to see what would happen if a string only containing numbers was entered.
I expected the output to wrap around the numbers each time the limit was reached, creating a new line each time.
On this occasion the output matched what I expected.

Test 3:
This test was to assess how the program would handle a word that was longer than the wrap limit.
I expected the word to be split across different lines where the wrap limit was reached.
The actual output was a traceback error, stating the substring had not been found. I repeated this test without the colon in the text input to see if that made a difference, but it did not.

Test 4:
In my fourth test I wanted to examine a really short wrap limit to see how the program would behave.
I was expecting the wrap limit to break the text input up across multiple lines.
The actual output was again a traceback error stating that the substring was not found.

Test 5:
This test was included as one that I expected to return no errors and not behave in an unexpected way.
I entered a sentence as the input and expected it to be broken across three lines by the wrap limit.
The actual output was similar to what I had expected, except for the fact I had misused the wrap limit in my initial write up of the tests.

Test 6 & 7:
These were the first two of my extended tests, looking at how the program would behave if a non-numerical wrap limit was entered.
In the first test I tried using a letter as the wrap limit and in the second I used punctuation, on both occasions expecting an error to be returned.
Both did return errors, but surprisingly (to me at least) they were different errors. The first was a value error stating that the limit needed to be an integer, but the second was an index error.

Tests 8 & 9:
These tests were to demonstrate the issues I originally had when I had thought that the program was not working as intended. I realised that it was due to my own error in misreading the guidance, but thought it was useful to demonstrate the errors that could occur from a user misunderstanding how the program should work.
The first test was to show what would happen if no wrap limit was provided and the second was to show what happened if no input at all was given. On each occasion I was expecting an error (as I had already seen them in a previous attempt).
Each time they generated an index error as expected and confirmed that the program required both a wrap limit and text input to be provided. I believe this shows that correct use of a program will usually be reliant on users correctly using and understanding instructions on how to work the program, otherwise errors are likely to be experienced.