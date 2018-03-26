# Making Your Own Block

**On this page, **you will create a new![](https://bjc.edc.org/bjc-r/img/1-introduction/gossip-response.png "gossip response")block that will make the program feel more like a conversation by using phrases like "I heard," "Who cares!" or "Well, guess what" instead of always "Oh, but." ![](https://bjc.edc.org/bjc-r/img/1-introduction/gossip2-reporting.png "gossip2 reporting &apos;Guess what. Gabrielle helped Señora&apos;")

#### For You To Do

1. If it isn't open already, open your U1L2-Gossip project.
2. Create the![](https://bjc.edc.org/bjc-r/img/1-introduction/gossip-response.png "gossip response") block. Instructions are below.

   **Making a New Block**

3. **Click **![](https://bjc.edc.org/bjc-r/img/1-introduction/make-a-block.png "make a block button") **in the Variables palette**, or **Control-click**\(or right-click\) in an empty spot in the scripting area and choose "make a block..." ![](https://bjc.edc.org/bjc-r/img/1-introduction/make-a-block.jpg "make a block option")

4. **Choose the color**, in this case red for Lists.

5. **Type the title** for your block: ![](https://bjc.edc.org/bjc-r/img/1-introduction/gossip-response.png "gossip response").

6. **Select the shape and click OK.** For this block, choose the oval _reporter_ shape because you want it to _report_ a value\(the chose response\) to another block\(the join\).![](https://bjc.edc.org/bjc-r/img/1-introduction/U1ImageVideoAddendum_img/U1GossipMakeABlock.gif)

**Coding the Block's Script**

1. **Drag in the blocks you need. **For this block, use ![](http://bjc.edc.org/bjc-r/img/1-introduction/list.png "the list block") and ![](http://bjc.edc.org/bjc-r/img/1-introduction/item.png "the item block").

2. **Snap the blocks together. **The code structure will look similar to`who`,`does what`, and`who2`.

3. **Fill any inputs**.

   1. For this project, click the down-arrow in `item `to change "1" to _random_.

   2. Then fill `list `with phrases

4. **Click OK **when you're satisfied.

![](/assets/pair_programming.png)

#### Vocabulary

In _most programming languages, what Snap_! _calls a reporter_\(blocks with an oval shape like![](http://bjc.edc.org/bjc-r/img/blocks/pick-random-empty-args.png "pick random \(\) to \(\)")\) is called a **function **and what Snap_! calls a command_\(blocks with a puzzle shape like![](http://bjc.edc.org/bjc-r/img/blocks/point-in-direction-90.png "point in direction \(90\)")\) is called a **procedure**. But programming languages are not consistent about this. Some use "function" for both, and others use "procedure" for both. \(Also, most languages use these words only for procedures or functions that you write, not the ones that are built into the language.\)

**The AP Exam uses the word **_**procedure **_**for both reporters and commands.**

```
  Note: Mathematicians use the word "function" in a slightly different way from computer scientists. Don't worry if you hear   something in math class that differs from what you see in BJC.
```

### Debugging

1. **Test **your custom `gossip response `block by clicking it several times. It should behave like the `who`,`does what`, and `who2`

   blocks.

2. **Debug** any problems before moving on.

3. **Use **your new block. Edit `gossip2`, and insert `gossip response `in place of the text "Oh, but...." ![](http://bjc.edc.org/bjc-r/img/1-introduction/gossip2-definition.png "gossip2 block definition with gossip response block inside")

4. **Test** and **debug** `gossip2 `also.

5. Then **test the whole program **by clicking script D several times , and **fix any bugs**.

![](/assets/save.png)

#### Take It Further

Edit `gossip `and `gossip2 `so that sometimes, not too often, they say something like "John and Paul" using two of the names in the lists of `who `or  `who2`.

* You can use code like![](http://bjc.edc.org/bjc-r/img/1-introduction/maybe.png "if \(\(random from 1 to 10\)&amp;gt; 7\)")
  to do something some of the time. Change the 7 to another number to adjust the probability.
* If your program uses two names at the beginning of the sentence, you'll have to use a plural verb instead of a singular verb. You can have two versions of `does  what `with different lists, or you can try to take a verb reported by `does what `and use an _algorithm_\(a series of steps, like a recipe\) to turn it into a plural verb.



