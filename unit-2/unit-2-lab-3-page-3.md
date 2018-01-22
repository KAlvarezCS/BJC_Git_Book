# Solving a Word Puzzle

**On this page**, you will solve a crossword puzzle by combining predicates using the`and`block. You will then use the resulting predicates with`keep`to find words with specific characteristics.

![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-example-5.png "keeping words with 6 letters with 1st letter r and 3rd letter b")

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L3-WordPuzzleSolver.xml) Run imports words list to initialize the words list variable.
2. You have used the ![](http://bjc.edc.org/bjc-r/img/blocks/length-of-blank-operator.png "length of \(\)") block in the Operators palette together with`= `and `keep `to find words of a certain length in the words list.

   1. Reassemble that script so that you can find all the words that have 8 letters.
   2. Find all the words that have 11 letters.
   3. You now have an _expression _that you can edit to test any word for any number of letters. This is a useful tool to have. Create and test a predicate _block _that takes a word and number as input and works like this:![](http://bjc.edc.org/bjc-r/img/2-complexity/does-orange-6-letters-true.png "does \(orange\) have \(6\) letters? reporting true")

      ![](http://bjc.edc.org/bjc-r/img/2-complexity/does-apple-7-letters-false.png "does \(apple\) have \(7\) letters? reporting false")

3. Build an _expression _using the ![](http://bjc.edc.org/bjc-r/img/blocks/letter-blank-of-blank.png "letter \(\) of \(\)") block with `= `and `keep `to find words that have certain letters in certain places.

   1. Use it to find all the words that begin with the letter i.

   2. Find all the words whose fourth letter is r.

   3. If you have not yet turned your expression into a predicate block, do that now. your block should work like this: ![](http://bjc.edc.org/bjc-r/img/2-complexity/is-letter-4-of-carrot-o-reporting-false.png "is letter \(4\) of \(carrot\) the letter \(o\)? reporting false")

      ![](http://bjc.edc.org/bjc-r/img/2-complexity/is-letter-2-of-giraffe-i-reporting-true.png "is letter \(2\) of \(giraffe\) the letter \(i\)? reporting true")

4. **Working with another pair.** use your predicates along with and and keep, to solve [this word puzzle](https://drive.google.com/open?id=1x8ShDe58qUQJDK8n97xoQGY4J4rw9aDsJCmkY-6SQc0).

   1. For example, this expression searches for 6 letter words that start with r and have b as the third letter:

      ![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-example-5.png "keeping words with 6 letters with 1st letter r and 3rd letter b")

[![](http://bjc.edc.org/bjc-r/img/2-complexity/crossword.jpg "word puzzle")](https://drive.google.com/open?id=1x8ShDe58qUQJDK8n97xoQGY4J4rw9aDsJCmkY-6SQc0)

#### Take It Further

1. Create and test a predicate block that checks whether a certain letter is in a word. Examples below. Your block should:
   1. Accept two inputs: a letter to check for and a word, and
   2. Report whether or not the inputted word has the inputted letter.![](http://bjc.edc.org/bjc-r/img/2-complexity/is-w-in-boston-reporting-false.png "is there a \(w\) in \(Boston\)? reporting false")
      ![](http://bjc.edc.org/bjc-r/img/2-complexity/is-w-in-new-york-reporting-true.png "is there a \(w\) in \(New York\)? reporting true")



