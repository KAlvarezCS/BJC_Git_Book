## Importing `Greet Player`into Another Program

Often you will find a use for code that you've already built in some other project.

**On this page, **you will transfer your `greet player`script into your Number Guessing game so you can use it there.

#### For You To Do

1. Open your U1L2-GreetPlayer project, run it a few times, and review the code so you remember how it works. \(Once you have some names in the player list, try names that are on the list and names that are not.\)

2. Fix any problems with `greet player`. When it's working correctly, export it. \(Instructions below.\)**Exporting Blocks**

   1. **Choose "Export blocks..." **from the Snap! file menu \(![](http://bjc.edc.org/bjc-r/img/1-introduction/file_button.png "File menu button")\).

   2. **Select only the block\(s\) you wish to export **\(in this case, just `greet player`\), and click "OK." An XML file will download.

3. Now, open your U2L1-NumberGuessing project, and import your `greet player`block. **Importing Blocks**

   1. **Choose "Import..." **from the Snap! file menu \(![](http://bjc.edc.org/bjc-r/img/1-introduction/file_button.png "File menu button")\).

   2. **Locate the XML file you exported **\(perhaps on your desktop or in your downloads folder\) and **click Open**.

   3. **Find the block\(s\) **you want. They will appear at the end of the palette that contains them.

   4. **Click the imported block to make sure it runs properly. **\(You'll likely see an error message after you've entered a name.\)![](http://bjc.edc.org/bjc-r/img/1-introduction/greet-player-error.png "greet player reporting an error message: &apos;Inside: Error. a variable of name &apos;player list&apos; does not exist in this context&apos;")

4. ![](/assets/talk_with_partner.png)Look at the code for `greet player`. Can you determine what's wrong?

#### Debugging Dependencies

Sometimes when you take a script out of the program where you built it and try to use it somewhere else, something breaks. It could be that the script depends on a custom block that isn't defined in the new program, or it could be \(as in this case\) that the script depends on a global variable that isn't defined in the new program.

To fix this problem so you can use the imported block, you'll need to define the global variable in your new program. Dependencies are one reason to use script variables rather than global variables whenever you can. Because they are defined in their scripts, you don't lose them when you move the script to a new place.

#### For You To Do

1. Create the missing global variable, player list, and make the program initialize it as an empty list.

   1. To make an empty list, click the left arrow on the list block so that there are no input spaces. ![](http://bjc.edc.org/bjc-r/img/2-complexity/set-to-empty-list.gif)If player list is initialized every time the game starts again, the game won't be able to remember any names. So, you will need to use a different event to start the game than to initialize player list. For example, you could use the green flag to initialize the list and use the space bar to begin the Number Guessing game.

2. **Test and Debug. **Your program should:

   * Greet the player and remember player names
   * Play the Number Guessing game with a new secret number every time

   Fix any problems with your code.

Is there a problem with the variable?

* Check the variable initialization \(where it is initially created\): Is the code where it needs to be? Does it do what you intend?
* Check the variable implementation \(where it is used\): Are you calling the variable you intend to? Are you using it how you intend to?

![](/assets/save.png)

