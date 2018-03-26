## Modeling Language: Plurals, Part 2

You can improve `plural `to work correctly with more words. If the project is not already open, please reload it. \(The suggested file name was `U2-Plural`.\)

#### For You To Do

1. **Abstraction: **Make a ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_h.png "plural-h") block that "specializes" on just one category, words that end with the letter **h**.

   1. Start with a `list `of the words you want it to work for.

   2. This specialist block should work correctly for words that fit its specialty ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_h-crutch-with-result.png "plural \(for words ending with h\) with correct  result for the word crutch")![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_h-moth-with-result.png "suffix s \(for words ending in h\) with result for moth"), ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_h-bush-with-result.png "plural \(for words ending in h\) with result"). It can be completely wrong about words that don't fit its specialty ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_h-mouse-with-%28wrong%29result.png "plural \(for words ending with h\) with wrong result for mouse \(wrong input\)")because the `plural `block should never give words to `plural-h `unless those words end with **h**.

   3. Test ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_h.png "plural-h") with a variety of words to make sure it works the way you want. Then use `map `to test it on the entire `list `you made earlier.

   4. **Abstraction:**Language often has special cases. In English, the plurals of some nouns add_s_; some add _es_; nouns like _calf and fly become calves and flies_, changing their final letters before adding _es_. And more. For a programming task this complex, it's \(generally\) best to break it into parts, handle each part separately with its own procedure \(its own block\), and then have the "top-level" block—in this case,`plural`, itself—use those specialists. That is, instead of coding every little detail directly in `plural`, it is cleaner and clearer to make `plural `look something like this.

      ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-abstract-definition.png "abstract definition of plural: if h = last letter of word, report h-case plural; if y = last letter of word, report y-case plural; if some other case, use a block that specializes in that case; etc.; else report join word s")

      Showing the structure of the method—just the overall strategy—in the "top-level" block and leaving the details to separate blocks is one part of an important computer science idea called **abstraction**. Abstraction keeps your code clear, readable, and more easily debugged. It will also help your code be more flexible.

2. When you trust your new specialist block, edit `plural `to use the specialist. Test \(you can use `map`\) to make sure `plural `still works for all the words it used to work for, as well as the new ones.

3. Create `plural-y `to handle words like ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_y-tray-with-result.png "plural\_y-tray-with-result")and ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural_y-sky-with-result.png "plural\_y-sky-with-result")

   1. Remember, any specialist can make mistakes if it's asked to do a job that isn't its specialty. Make sure `plural `gives it only the job it knows how to handle correctly.

![](/assets/save.png)

#### Take It Further

1. Because you know what ![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-items-such-that-%28last-letter-of-%28input%29-equals-h%29-from-test-list.png "keep-items-such-that-\(last-letter-of-\(input\)-equals-h\)-from-test-list") does, you can, if you like, use just that specialized list as input to a test of plural or plural-h, this way. ![](http://bjc.edc.org/bjc-r/img/2-complexity/map-plural%28with-input%29-over-%28keep-items-such-that-%28last-letter-of-%28input%29-equals-h%29-from-test-list%29.png "map-plural\(with-input\)-over-\(keep-items-such-that-\(last-letter-of-\(input\)-equals-h\)-from-test-list\)")

2. Extend `plural `to handle another special case. Use a special-purpose block for your special case to keep `plural`from becoming cluttered.

3. Right now, if `plural `is given a word with a space at the end, it leaves that space in the plural, like this: ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-bulldog[space]-with-result%28bulldog[space]s%29.png "plural of bulldog with space at the end, and result with space before s") . Figure out how to handle this special case and edit `plural `so that the result is ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-bulldog[space]-with-result%28bulldogs%29.png "plural of bulldog with space at the end, and correct result, no space before s"). You already have a block that specializes in making plurals of words that don't have a space at the end. Use it.

4. **Surprise! **Once `plural `works for a single space at the end of a word, try giving it ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-bulldog[four-spaces].png "plural of bulldog with four spaces at the end"). That works!! But why?!

![](/assets/save.png)

