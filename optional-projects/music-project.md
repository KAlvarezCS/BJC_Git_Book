# Music Project

**In this project,**you will use the Snap_!_`play note `block to create music while you review abstract data types and higher order functions.

#### For You To Do

1. Start a new project. Save it as "U3-MusicProject"
2. ![](https://bjc.edc.org/bjc-r/img/icons/headphones.png "Set Up Your Headphones or Speakers")
3. ![](https://bjc.edc.org/bjc-r/img/icons/import-tools.png "Import Tools")

## Reviewing Higher Order Functions With Sound

#### For You To Do

1. Build and compare these `play `scripts. Run each script a few times.

   1. ![](https://bjc.edc.org/bjc-r/img/3-lists/compare-play-note-1.png "play note \(item \(any\) of \(list \(60\) \(64\) \(67\) \(72\) \(60\)\)\) for \(1\) beats")
   2. ![](https://bjc.edc.org/bjc-r/img/3-lists/compare-play-note-2.png "for each \(note\) of \(list \(60\) \(64\) \(67\) \(72\) \(60\)\) \(play note \(note\) for \(1\) beats\)")
   3. ![](https://bjc.edc.org/bjc-r/img/3-lists/compare-play-note-3.png "for each \(note\) of \(map \(\_ + 5\) over \(list \(60\) \(64\) \(67\) \(72\) \(60\)\)\) \(play note \(note\) for \(1\) beats\)")
   4. ![](https://bjc.edc.org/bjc-r/img/3-lists/compare-play-note-4.png "for each \(note\) of \(keep items such that \(\(\) &amp;lt; 65\) from \(list \(60\) \(64\) \(67\) \(72\) \(60\)\)\) \(play note \(note\) for \(1\) beats\)")

   Need To Review?  
   1. You Learned about for each in [Unit 2 Lab 2](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/2-data-structures-art/1-the-for-each-block.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment).  
   2. You learned about keep in [Unit 2 Lab 3](https://bjc.edc.org/bjc-r/cur/programming/2-complexity/3-predicates/2-keeping-list-items.html?topic=nyc_bjc%2F2-conditionals-abstraction.topic&course=bjc4nyc.html&novideo&noassignment).  
   3. You learned about map in[ Unit 3 Lab 1](https://bjc.edc.org/bjc-r/cur/programming/3-lists/1-introduction-to-lists/4-mapping-over-list.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment).

## Creating an Abstract Data Type to Organize Musical Data

#### For You To Do

1. Create a `note `ADT to manage the pitch and length of each note in a song.

   1. \_Pitch\_is the amount of highness or lowness of a musical note; the pitch value goes in the first input slot of the `play note `block.

      The \_length \_of a note is the amount of time that the note plays \(the number of beats\); the length value goes in the second slot of `play note`.

      1. Create the constructor ![](https://bjc.edc.org/bjc-r/img/3-lists/note-constructor.png "note, pitch: \(\) length: \(\)")

      2. Create two selectors: ![](https://bjc.edc.org/bjc-r/img/3-lists/note-selector-pitch.png "pitch from note: \(\)") ![](https://bjc.edc.org/bjc-r/img/3-lists/note-selector-length.png "length from note: \(\)")

![](/assets/save.png)

## Creating Blocks to Play Music

#### For You To Do

1. Use `for each `together with your selectors to build a ![](https://bjc.edc.org/bjc-r/img/3-lists/play-song-block.png "play song {}") block that takes a list of notes as input and plays each pitch for the specified number length of time. ![](https://bjc.edc.org/bjc-r/img/3-lists/play-song-data-type.png "Play Song data type definition")[Click here for a chart for note pitch numbers.](https://bjc.edc.org/bjc-r/cur/programming/3-lists/optional-projects/3-music-project.html?topic=nyc_bjc%2F3-lists.topic&course=bjc4nyc.html&novideo&noassignment#hint-target)

2. Create a reporter to reports the notes for a song of your choosing. Here's an example: ![](https://bjc.edc.org/bjc-r/img/3-lists/row-row-row-reporter.png "row row row your boat reporter block definition")

3. Test your song with your `play song `block, and debug any problems. ![](https://bjc.edc.org/bjc-r/img/3-lists/play-song-row-row-row.png "play song \(row row row your boat\)")

#### If There Is Time...

1. Use the ![](https://bjc.edc.org/bjc-r/img/3-lists/set-tempo-to-empty.png "set tempo to \(\) bpm") block to change the pace at which the notes are played. A higher number will make your song play faster; a lower number will make it play slower.

   1. BPM stands for "beats per minute."

## Transposing Music

#### For You To Do

1. Compare the output of these two scripts that you created above. Discuss what `map + 5 `does to the sounds you hear: ![](https://bjc.edc.org/bjc-r/img/3-lists/compare-play-note-2.png "for each \(note\) of \(list \(60\) \(64\) \(67\) \(72\) \(60\)\) \(play note \(note\) for \(1\) beats\)")

   ![](https://bjc.edc.org/bjc-r/img/3-lists/compare-play-note-3.png "for each \(note\) of \(map \(\_ + 5\) over \(list \(60\) \(64\) \(67\) \(72\) \(60\)\)\) \(play note \(note\) for \(1\) beats\)")

2. Use `map `together with your ADT blocks to create a reporter that transposes \(shifts\) a list of notes. It should take a list of notes and a number indicating how much to transpose \(shift\) the song as input, and it should report the adjusted song. For example: ![](https://bjc.edc.org/bjc-r/img/3-lists/play-song-transpose-row-row-row-by-19.png "play song \(transpose \(row row row your boat\) by \(19\)\)")

3. Try playing your song using your transpose block with several different shift numbers so that you can hear_ the impact of map._



