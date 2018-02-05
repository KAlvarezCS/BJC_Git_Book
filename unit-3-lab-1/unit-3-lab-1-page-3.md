# Selecting Specific Data

**On this page, **you will develop code for a "Find Contact" button to locate contacts in the list.![](http://bjc.edc.org/bjc-r/img/3-lists/find-contacts-with-name-Alphie-reporting.png "find contacts with name: \(Alphie\) reporting")

As you add more contacts to your list, it will become less and less realistic to find the one you want by reading through the whole list. So building a search feature will become essential for finding the desired information efficiently. Lists, adding and removing items from lists, and searching lists are common features in many programs.

#### For You To Do

1. If it isn't open already, open your U3L1-ContactList project.
2. Write a ![](http://bjc.edc.org/bjc-r/img/3-lists/find-contacts-with-name.png "find contacts with name: \(\)") block that takes a text string as input and reports either a list of the contacts whose name includes that string or an empty list if no such name is in contact list.

   1. **Use these blocks:**

      1. ![](http://bjc.edc.org/bjc-r/img/3-lists/string-contains.png "string \(\) contains \(\) ?"), which reports `true `if the first string \(for example, a contact's name in the list\) contains the second string \(for example, a name or part of a name\)

      2. ![](http://bjc.edc.org/bjc-r/img/blocks/keep.png "keep items such that &amp;lt;&amp;gt; from \(list\)"), which reports only the items that make the function true

      3.  ![](http://bjc.edc.org/bjc-r/img/blocks/empty.png "empty {} ? predicate function"), which returns `true `if the list is empty and `false `otherwise

      4. Selector ![](http://bjc.edc.org/bjc-r/img/3-lists/name-selector.png "name from contact: \(\)")

3. Develop a "Find Contact" button.

   1. Make the script ask the user whose contact to search for and have the sprite `say `each of the matching contacts.
   2. If the contact is not in the list, make the sprite say "not found."

4. **Debug.** Make sure everything works the way you want it to before going on.

![](/assets/save.png)

#### If There Is Time...

1. Develop a "Delete Contact" button.

   1. Move the "Delete Contact" button onto the stage.
   2. Make the script ask the user to "Enter the name of the contact\(s\) you wish to delete."
   3. Then, use your `find contacts `block to find all the matching contacts.

   4. Give the user the list of matching contacts and ask them for confirmation to delete \(so the user won't accidentally delete their contact\).
   5. If the user confirms that they want to delete these contacts, replace the contact list with a list of all contacts whose name does not match the inputted name.

2. Modify your "Delete Contact" script so that it lets the user choose which contact they want to delete when`find`

   reports more than one.



