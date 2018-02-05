# Transforming Every List Item

**On this page,**you will use your ADTs with the `map `block to display all the names in your contact list.

As you know, the

`keep`

block allows you to check every item in a list using a predicate, and it reports only the items that make the predicate true. The![](http://bjc.edc.org/bjc-r/img/blocks/map.png "map") block also lets you work across a whole list at once. `Map `allows you to perform the same function on every item of a list. `Map `takes two inputs: a function \(a reporter with a blank input slot\) and a list, and it reports a new list. Every item in this new list is the result of calling the function with an item from the original list as input. For example:

![](http://bjc.edc.org/bjc-r/img/3-lists/map-example-2.png "map \(join \( \) \(s\)\) over \(list \(cat\) \(dog\) \(bird\)\) reporting")

![](http://bjc.edc.org/bjc-r/img/3-lists/map-example-3.png "map \(round \( \)\) over \(list \(3.14159\) \(87\) \(5.4\)\) reporting")

You write the function that describes the change, and`map`applies that function to each item in the input list and then reports the list of values reported by the function.

Notice that the function mapped over the list always has a blank input slot. With both`map`and`keep`that blank is required. This blank is where the list item goes each time the function is performed.

#### For You To Do

1. If it isn't open already, open your U3L1-ContactList project.
2. ![](/assets/talk_with_partner.png) Experiment with these examples of map. discuss and then explain in writing what these expressions are doing.![](http://bjc.edc.org/bjc-r/img/3-lists/map-join-s.png "map \(join \( \) \(s\)\) over \(list block script Boolean\)")
   ![](http://bjc.edc.org/bjc-r/img/3-lists/map-3x.png "map \(\(3\) \* \( \)\) over \(list 7 8 1\)")

   ![](http://bjc.edc.org/bjc-r/img/3-lists/map-letter-1.png "map \(letter 1 of \( \)\) over \(list bounce join clear\)")

3. Use the `map `block together with your constructors to report a list of only the names of all contacts.

Like the `keep `block, `map `isn't installed automatically. It has already been added to this project, but in other projects, you'll need to select "Import tools" from the File menu to access the `map `block.

