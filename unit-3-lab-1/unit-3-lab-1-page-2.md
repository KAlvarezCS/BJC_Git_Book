.Adding Contact Data

**On this page, **you will develop code for "Add Contact" and "Clear List" buttons in your contact list program.

#### For You To Do

1. If it isn't open already, open your U3L1-ContactList project.
2. Develop the "Add Contact" button for the user.

   1. Make the script ask the user for contact data and then add that data to the contact list using the contact constructor.

   2. **Collecting Data from the User:  **You'll want to ask the user for each piece of data \(contact name, address, and phone number\) separately.

      1. **You **_**could **_**use several `ask `and `answer `blocks together with script variables **to request and then store each piece of user input until you are ready to report them all together using `contact`.  ![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-with-variables.png "contact with name: \(name\) address: \(address\) phone: \(phone\)")

      2. _**Another way **_**that makes for cleaner code is to use **_**abstraction**_**: create helper blocks **\(such as ![](http://bjc.edc.org/bjc-r/img/3-lists/ask-name.png "ask name") and ![](http://bjc.edc.org/bjc-r/img/3-lists/ask-phone.png "ask phone")\) that each ask the user for one piece of data and report their answer to the `contact `constructor.![](http://bjc.edc.org/bjc-r/img/3-lists/contact-constructor-with-helpers.png "contact with name: \(ask name\) address: \(ask address\) phone: \(ask phone\)")

      3. Each of these helper blocks will `ask `the user a specific question \(like, "What is the contact's address?"\) and then report the user's `answer`.

         1. You could first build a more general![](http://bjc.edc.org/bjc-r/img/3-lists/answer-to-prompt.png "answer to prompt \(\)")helper block \(yet another abstraction\) to use in the other helper blocks instead of rewriting the `ask `and `answer `script every time.

   3. **Test and debug.** Add a few made-up people to your contact list. Make sure everything works.

      1. You can use these examples or make up your own:

         | name | address | phone |
         | :--- | :--- | :--- |
         | Betsy Anderson | 123 Main St. \#4, New York, NY 10001 | 212-555-1234 |
         | Alphie Preston | 149 E. 16th Ave., Sunnyvale, CA 94089 | 208-555-6789 |
         | Gamal Abdel | 369 Center St., Boston, MA 02130 | 617-555-1098 |

3. Develop a "Clear List" button that resets the contact list to an empty list.

   1. Make the script ask the user for confirmation \(so the user won't accidentally delete their list\).

      1. For example, clicking, "Clear List" might `ask `the user, "Enter c to clear the list, or enter anything else to cancel."

   2. **Debug.** Make sure this feature behaves as expected for either user choice. 

#### ![](/assets/save.png)

#### If There Is Time...

1. The sprites' questions might be covered up by the contact list watcher on the stage. Use `hide variable `and `show variable `to hide the contact list watcher until the end of each sprite's script.



