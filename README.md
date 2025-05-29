# COP-4020-Homework-4-solution

Download Here: [COP 4020 Homework 4 solution](https://jarviscodinghub.com/assignment/cop-4020-homework-4-solution/)

For Custom/Original Work email jarviscodinghub@gmail.com/whatsapp +1(541)423-7793

Problem 1:
———-

Implement the function

nTimes :: Integer -> Parse a b -> Parse a [b]

so that nTimes n p recognizes n of the objects recognized by
the parser p.

This problem is exercise 17.11 of the book “Haskell – the craft
of functional programming”. I have already solved exercise 17.10;
check out the code in Parser.hs following the comment
“– begin: helper parsing functions” to help you solve this problem.

Problem 2:
———-

Implement the function

spotWhile :: (a -> Bool) -> Parse a [a]

whose parameter is a function which tests elements of the input type, and
returns the longest initial part of the input, all of whose elements have
the required property. For instance,

spotWhile isDigit “234abc” == [(“234″,”abc”)]
spotWhile isDigit “abc234″ == [([],”abc234”)]

Problem 3:
———-

Modify the function

parser :: Parser Char Expr

defined in the file ExpressionsParser.hs so that the whitespace characters
space and tab can be used in expressions, but are ignored on parsing.
(Hint: there is a simple pre-processor which does the trick!)

This is exercise 17.18.

Problem 4:
———-

Implement the function

merge :: Store a b -> Store a b -> Store a b

that takes two stores as input and produces the corresponding
“merged” store as output. Note that there are four
possibilities: a key could be contained in

a) none of the two stores
b) only the first store
c) only the second store
d) both stores.

In case d), the first store has priority, that is, the merged
store should contain the value from the first store.

Submission instructions:
————————

You have to modify the three files:

– Parser.hs (Problem 1 and 2)

Add your solutions above the comment “– end: helper parsing functions”.

– ExpressionsParser.hs (Problem 3)

Modify directly the parser function. You may want to add the
pre-processing function outside the modified parser function.

– Store.hs (Problem 4)
Add your solution at the end of the file and make sure that
you export the merge function.

Make sure that you run the tests.

Zip the three modified files and upload them to Webcourses.
