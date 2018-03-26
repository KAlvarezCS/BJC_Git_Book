# Analyzing and Improving Searches

**On this page**, you will see how the characteristics of a list can affect the algorithm for searching in it.

### Searching in Unsorted Data

Searching for an item in \_unsorted \_data is less efficient because you have to check every item, but it is easier to code.

#### For You To Do

1. Build a `position of number in unsorted list`block that reports the earliest location of a number in an unsorted list or reports "Not In List" \(or NIL, if you like\) if the number is not in the list. ![](https://bjc.edc.org/bjc-r/img/5-algorithms/position-of-number-12-in-unsorted-list-reporting-2.png "position of number \(12\) in unsorted list\(list{20,12,3,100,50,12}\) reporting 2")

   ![](https://bjc.edc.org/bjc-r/img/5-algorithms/unsorted-list.png "unsorted list {20, 12, 3, 100, 50, 12}")

Searching unsorted data can be incredibly slow if we're dealing with a lot of data, but it is fairly quick when working with short lists.

### Searching in Sorted Data

If you are searching for a number in a sorted list, you have more information. Suppose you have a sorted list and you want to locate the position of a number.

Typically, sorted lists are from lowest to highest. You'll create a block that sorts a list of numbers in Unit 8, [Sorting a List](https://bjc.edc.org/bjc-r/cur/programming/8-recursive-reporters/2-sorting/1-sorting-a-list.html?topic=nyc_bjc%2F7-recursive-reporters.topic&course=bjc4nyc.html&novideo&noassignment).

#### Thinking Out Loud

**Alphie:**  If the list is sorted, we could look at the middle element of the list and see if our number is in the first or last half of the list. That would save time.

**Betsy:** This feels a lot like the guessing game we built—I pick a number and the computer tries to guess it by splitting the list in half with each guess.

![](https://bjc.edc.org/bjc-r/img/5-algorithms/awful-list-indexed.png "awful-list {1:1, 1:7, 3:8, 4:9, 5:11, 6:12, 7:21, 8:22, 9:23, 10:24, 11:73, 12:73, 13:96, 14:99}")

**Alphie: **But in that one, the computer guessed a number that we picked. Now we want it to find a number in a list

and report its position. It should work like this:![](https://bjc.edc.org/bjc-r/img/5-algorithms/position-of-number-11-in-sorted-list-awful-list.png "position of number \(11\) in sorted list \(awful list\) reporting 5")

**Betsy:** Yes, but it still feels the same. It should have the same guts as the guessing game.

Betsy's last remark is a version of **abstraction**. Betsy noticed that `position in sorted list`and the [number guesser algorithm](https://bjc.edc.org/bjc-r/cur/programming/5-algorithms/1-searching-lists/1-sorted-lists.html?topic=nyc_bjc%2F5-algorithms.topic&course=bjc4nyc.html&novideo&noassignment) should have the same overall _structure._

#### For You To Do

1. Using the strategy of your guessing game project from the previous page, write a block that says:

   1. the position of an item in an ordered list, and,
   2. the number of guesses it takes to find the number
   3. ![](/blocks/saypos11.png)![](/assets/sayposresponse.png)

2. Then, build a `position of number in sorted list `block that returns the position of a number in a list sorted from lowest to highest or zero if the number is not in the list. \(Note: This task is identical to the previous one except that instead of the block "saying" the position it will need to "report" the position.\) ![](https://bjc.edc.org/bjc-r/img/5-algorithms/position-of-number-11-in-sorted-list-awful-list.png "position of number \(11\) in sorted list \(awful list\) reporting 5")

   ![](https://bjc.edc.org/bjc-r/img/5-algorithms/position-of-number-2-in-sorted-list-awful-list.png "position of number \(2\) in sorted list \(awful list\)  reporting 0")

#### If There Is Time...

1. Make a table that tracks the number of guesses it takes to find a number in a sorted list depending on the length of the list if that number turns out to be the last item.

| Length of List | Number of Guesses |
| :--- | :--- |
| 3 |  |
| 7 | 3 |
| 15 |  |
| 63 |  |
| 127 |  |



