## Creating the Contact ADT

**In this lab,**you will develop a Contact List database application like the one on your phone.

**On this page,**you will develop an **Abstract Data Type **to store and access _contact data_\(name, address, phone number, etc.\).

### Setting Up the Contact List

#### For You To Do

1. [Click here to load. Save to your Snap! account.](http://snap.berkeley.edu/snapsource/snap.html#open:http://bjc.edc.org/bjc-r/prog/3-lists/U3L1-ContactList.xml)
2. Create global contact list variable.

3. Initialize contact list as an empty list.

#### **Why global?**

**Multiple scripts **across the project **will use this variable **, so it shouldn't be attached to just one script like a local, script variable.

Also, in Snap_!_, only globals save their data when the project is saved.

### Creating the ADT

#### Thinking Out Loud

Betsy and Gamal are planning to build a Contact List in Snap_!_.

**Betsy:** We need a way to add a contact to our contact list.

**Gamal:** Each contact will be a list that with the a person's name, phone number, address, email, or whatever we write.

**Betsy:** In Unit 2, we created a [`point `abstract data type](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/2-data-types.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) to store the coordinates of each point in a list of points. Here, we can make a `contact `abstract data type to store the data for each contact in our list of contacts.

**Gamal:** Yes! _\(Gamal opens their old project, but you don't need to.\) _Before, we used a `point `constructor to construct a list of coordinates. 

Gamal points to the code for the `point `constructor: ![](http://bjc.edc.org/bjc-r/img/3-lists/point.png "point\(X\#\)\(Y\#\){report\(list\(X\)\(Y\)}")

**Betsy:** Then we used two selectors to select either the _x _or _y _coordinate.

Betsy points to the code for the `coordinate `selectors: ![](http://bjc.edc.org/bjc-r/img/2-complexity/xcor.png "x coordinate of \(point\); report item 1 of \(point\)")

and ![](http://bjc.edc.org/bjc-r/img/2-complexity/ycor.png "y coordinate of \(point\); report item 2 of \(point\)")

**Gamal:** In this project, we'll need a `contact `constructor and selectors to access the name, address, and phone number for any given contact.



#### For You To Do

1. Create a `contact `_constructor _that accepts three pieces of data as input: the contact's name, phone number, and address.

   1. ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-untyped.png "contact name: \(\) address: \(\) phone: \(\)") It should report one whole contact \(a list of the three items\):  
      ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-reporting.png "contact name: \(Betsy\) address: \(123 Main St. \#4, New York, NY 10001\) phone: \(212-555-1234\) reporting {Betsy Anderson; 123 Main St. \#4, New York, NY 10001; 212-555-1234}")

2. Write the _selector _blocks to retrieve the `name from contact`, `address from contact`, or `phone from contact`: ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-in-name-selector.png "contact name \(contact block with inputs\) reporting ")  
   ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-in-address-selector.png "contact address \(contact block with inputs\) reporting ")  


   ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-in-phone-selector.png "contact phone \(contact block with inputs\) reporting ")

3. Declare input types for each selector to make it obvious that they expect a list \(one whole contact\) as input. ![](http://bjc.edc.org/bjc-r/img/3-lists/name-selector.png "name from contact: \(\)") ![](http://bjc.edc.org/bjc-r/img/3-lists/address-selector.png "address from contact: \(\)") ![](http://bjc.edc.org/bjc-r/img/3-lists/phone-selector.png "phone from contact: \(\)")

   1. You learned about [Specifying an Input Type](http://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/1-the-for-each-block.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment) in Unit 2.

You will use your contact ADT blocks to build your contact list, so debugging them before you continue will help ensure that your final project works correctly.

#### For You To Do

1. Test your blocks together, and debug any problems.

   1. First, put the constructor \(with input values\) inside each selector \(as shown above\) to test that they each report the correct piece of data.
   2. Then, use the `contact `constructor to `add `a few contacts to your contact list.

      1. You can use these examples or make up your own:

         | name | address | phone |
         | :--- | :--- | :--- |
         | Betsy Anderson | 123 Main St. \#4, New York, NY 10001 | 212-555-1234 |
         | Alphie Preston | 149 E. 16th Ave., Sunnyvale, CA 94089 | 208-555-6789 |
         | Gamal Abdel | 369 Center St., Boston, MA 02130 | 617-555-1098 |

   3. Notice how your contacts appear in the list.
      1. Snap_! _has two different views for lists within lists. You can switch which view you see by right-clicking \(or control-clicking\) on the contact list watcher on the stage.

      2. If you don't see the watcher on the stage, make sure the checkbox beside the contact list variable in the Variables palette is checked. ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-list-watcher.png "contact list watcher checked")

      3. **Table View **for Contact List Watcher: ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-list-table-view.png "contact list watcher in table view")
   4. **List View **for Contact List Watcher: ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-list-list-view.png "contact list watcher in list view")

2. Try selecting the `name`,`address,` or `phone `from a contact in your list ![](http://bjc.edc.org/bjc-r/img/3-lists/name-from-contact-random-reporting.png "name from contact: \(item \(random\) of \(contact list\)\) reporting Alphie Preston")

3. **Debug** any problems.







