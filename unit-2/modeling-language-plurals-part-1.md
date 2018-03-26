## Modeling Language: Plurals, Part 1

Siri and other robots are programmed to generate language. Siri speaks; some robots write. You have developed a program, `gossip`, that writes. Now, you can extend the computer's abilities with language by developing a reporter block, `plural`, that takes a noun as input and correctly spells and outputs the plural.![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-day-with-result.png "plural day \(with result\)")![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-boss-with-result.png "plural boss \(with result\)")

Spelling a plural can seem almost automatic for a person, but it is not simple: a computer needs an algorithm to do that task.

#### For You To Do

1. To do this project, you will need to use the new blocks ![](http://bjc.edc.org/bjc-r/img/2-complexity/last-letter-of-169x27.png "last letter of"), and ![](http://bjc.edc.org/bjc-r/img/2-complexity/all-but-last-letter-of-231x27 pixels.png "all but last letter of"). You will also need ![](http://bjc.edc.org/bjc-r/img/2-complexity/%28list-of-items%29-contains-%28some-item%29-predicate.png "\(list-of-items\)-contains-\(some-item\)-predicate") and ![](http://bjc.edc.org/bjc-r/img/2-complexity/join-117x27.png "join"), which you used in Unit 1 Lab 2, Gossip and Greet. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/2-complexity/U2-project-plural.xml) Try all its expressions \(the nine one-line scripts\) and experiment with their inputs until you are sure you understand what they do. For each expression, say what that script does

   _in general not just what it does with this particular input. \(Example: _![](http://bjc.edc.org/bjc-r/img/2-complexity/last-letter-of-butterfly-with-result-y.png "last-letter-of-butterfly-with-result-y")_reports y_, but you want to say what `last letter of `will report if, say, `2017 `is its input.\)

   1. You won't need ![](http://bjc.edc.org/bjc-r/img/2-complexity/join-t-all-but-first-letter-of-when-343x33.png "join-\(t\)-all-but-first-letter-of-when") this for the project, but you might find it interesting to try it not only with "when," as an input but with "where," "what," "wherefore." Linguists use evidence like this to understand the history of a language.

2. Here's one way to start building the `plural `block. Build this much and test it out on at least "day" and "boss" and "medicine," to make sure it works correctly for those. If it does not, edit and fix it. ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-%28script%29.png "plural-\(script\), first try")

   1. Choose the reporter button when you make `plural`.![](http://bjc.edc.org/bjc-r/img/building-blocks/make-a-reporter.png "select reporter as block type")

3. **Debugging: **Try to find words for which this version of `plural `does _not work correctly. List the words you find. Organize that list_, sorting the words into categories according to their last letter. For example, it will get wrong some words that end with the letter _h_. Try to find many words it gets wrong.

4. **Save to your list.**

   1. Create a Snap! list like this ![](http://bjc.edc.org/bjc-r/img/2-complexity/noun-list-for-testing-plural2.png "snap list block containing day, boss, bulldog\(with space at end\), box, butterfly, brush, and more of your choosing")containing all of your words.

   2. Save this as "U2-Plural" Save your file. You will need this list.

   3. **Debugging: **To write code that works, you want to try to find situations in which it does \_not \_work. "Breaking it" requires thinking of wild and exceptional cases, even including inputs that are incorrect in some way, like this example, which has a space at the end. ![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-bulldog[space]-with-result%28bulldog[space]s%29.png "plural of a word with a space following the word")

5. `plural `should now work correctly for "day" and "boss" and "medicine," but it probably doesn't yet work correctly for the word "box"![](http://bjc.edc.org/bjc-r/img/2-complexity/plural-box-with-%28wrong%29-result.png "suffix s box \(with wrong result\)"). Edit your `plural `block to make it work for words that end with x. Test it to make sure it does work properly.

![](/assets/save.png)

You can do the same for conjugating verbs in Spanish or some other language you choose. See the Take It Further section at the bottom.

The next two steps are worth learning—very useful for _testing _`plural `and in more advanced work later on—but not essential for _building _`plural`.

#### For You To Do

1. Use `map `to test all the words on your list. Leave the slot in `plural `**empty**, as you see here. The `map `block inserts each element of the list into that slot and reports a list of the results. ![](http://bjc.edc.org/bjc-r/img/2-complexity/map-plural-over-list-of-nouns.png "map-plural-over-list-of-nouns")

   For now, don't worry about the words it still gets wrong, as long as it works for "day," "boss," "medicine," and "box."

2. In your `map `script, replace `plural `with ![](http://bjc.edc.org/bjc-r/img/2-complexity/join-%28%29-y.png "join-\(empty\)-y"). Try it. Now explain what the `map `block does, _in general_.

3. Experiment with ![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-items-such-that-%28last-letter-of-%28input%29-equals-h%29-from-test-list.png "keep-items-such-that-\(last-letter-of-\(input\)-equals-h\)-from-test-list") and ![](http://bjc.edc.org/bjc-r/img/2-complexity/keep-items-such-that-%28last-letter-of-%28input%29-equals-y%29-from-test-list.png "keep-items-such-that-\(last-letter-of-\(input\)-equals-y\)-from-test-list") to see what they do.  Again, leave the slot in `last letter of `**empty**, as you see here. That is the placeholder for `keep `to test each word the list. Explain what the `keep `block does.

#### Take It Further

* If you know another language, build a block that takes a pronoun and verb as input and outputs the correct form of that verb. For example: ![](http://bjc.edc.org/bjc-r/img/2-complexity/conjugate-verb-%28spanish%29-for-nosotros-comer.png "conjugate verb \(Spanish\) for nosotros comer") ![](http://bjc.edc.org/bjc-r/img/2-complexity/conjugate-verb-%28spanish%29-for-yo-tocar.png "conjugate verb \(Spanish\) for yo tocar")



