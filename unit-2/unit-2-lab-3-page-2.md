# Keeping Items From a List

**On this page**, you will use predicates with the`keep`block to keep items in a list that have specific characteristics.

As you know, predicates can be used with conditionals to decide when to_do\_something; they can also be used with_`keep`_to decide which things to\_keep_. The![](http://bjc.edc.org/bjc-r/img/blocks/keep.png "keep")block takes a list and a predicateas input, and it reports a new list keeping only the items from the list that make the condition described by the predicate true.

For example, the following expression will find words from thewords list**whose first letter is v**. The\_blank input slot\_is where each item of the list goes to decide if it will be kept.  
![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-example-6.png "keep items such that \(\(letter\(1\) of \( \)\) = \(v\)\) from \(word list\)")

You write the predicate that does the checking, and`keep`**applies the predicate to each item in the input list and then reports the list of items that make your predicate**`true`.

Note that the blank input slot in the predicate is \_required \_when using `keep`. This is where the item from the list goes each time the question is asked.

#### For You To Do

[![](http://bjc.edc.org/bjc-r/img/icons/load-save.png "Click here to load this file. Then save it to your Snap! account.")](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2L3-KeepingData.xml)

1. [Export](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/1-variables-games/4-importing-exporting.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) your new predicates \( `between?`, `divisible?`, `even?`, and perhaps also`integer?`\) from
   [your U2L3-Predicates project](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/1-adding-questions.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) and then import them into the new project and save the new project.
2. ![](http://bjc.edc.org/bjc-r/img/icons/talk-with-your-partner.png "Talk with Your Partner") Experiment with these examples of `keep`. Discuss and then explain _in writing_
   what these expressions are doing.
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-example-4.png "keep items such that \(\(length of \( \)\) = \(5\)\) from {apple, banana, orange, grape, kiwi, mango, watermelon} reporting {apple, grape, mango}")
   ![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-example-7.png "keep items such that \(not\(is \(\) a \(number\)?\)\) from {5, :\), six, 7, elephant, 3} reporting {5,7,3}")

Like [the `for`block](http://bjc.edc.org/bjc-r/cur/programming/1-introduction/3-drawing/6-the-for-block.html?topic=nyc_bjc%2F1-intro-loops.topic&course=bjc4nyc.html&novideo&noassignment), `keep`isn't installed automatically. It has already been added to this project, but in other projects, you'll need to select "Import tools" from the File menu to access the `keep`block.

The first example keeps inputs of a certain _length_; every word in the list is asked whether its length is 5, and only those with five letters are reported. The second example keeps inputs that are _not numbers_; every item in this list is asked "Is this item \_not \_a number?" and only the elements that are not numbers are reported.

#### For You To Do

Run `initialize lists`, and then use your new predicates together with `keep`to answer these questions:

1. How many 12-letter words are in words list?
2. How many 15-letter words are in words list?
3. How many 17-letter words are in words list?
4. How many items in the numbers listare:
   1. Even?
   2. Between 25 and 75?
   3. Even numbers that are greater than zero?

#### If There Is Time...

If you created an `integer?`predicate, use your new predicates together with `keep`to determine how many numbers in the numbers list are:

1. Integers?
2. Integers between 25 and 75?
3. Not integers?
4. Odd integers?



