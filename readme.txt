Application usage and user's manual.


0. Installation

You have the application running, thus you have installed it successfully.. :)


1. Loading and saving griddlers.

To open a griddler, click the Load from File button and choose a file with saved griddler. To save a griddler back to file click the Save to File button and choose a file. Such saved grid-file always contain both the clues and the picture itself. That means that the file may be used for distributing unsolved griddlers as well as for saving partially or fully solved ones. Nonetheless, there are three different types of file extensions, just to determine what is saved inside. The user is encouraged to use the appropriate extension upon saving.

All distributed grid-files contain fully solved picture along with the clues. This is a solving application, thus no need to hide the solution from you. If you want to solve a griddler yourself, you will have to clear the picture first on your own. To run a solver and see how it is working, you will have to clear the picture as well. You may use the Automatically clear picture checkbox to clear every griddler you open. Note: Remember turning this option on! If you save a partially solved griddler to a grid-file, your partially solved picture will be saved into it. However, upon load, this checkbox will clear your picture.


2. Zooming

The griddlers comes in all different sizes. The application always tries to find the best zooming for the griddler, however, the user is encouraged to adjust it on his own as well. Usually there is no need to see all the clues and all the picture all the time. To zoom out, click the - button, to zoom in, click the + button. The 0 button between + and - is to reset the zooming to the default value.


3. Solving the griddler

After a griddler is loaded (and the picture is cleared), the user may start solving it. The rules and hints how to do that are described in the section of Rules and Hints.

All the griddlers in this application are monochromatic. Therefore they use only a foreground color and a background color.  The foreground color is represented with a box and is drawn as a square filling a cell. The background color is represented with a space and is drawn as a cross within a cell. Finally, some cells that are not yet decided whether are to be boxes or spaces in the picture are left empty.

To put a box in a cell, click on the cell with left mouse button. To put a space in a cell, click on the cell with right mouse button. If you make a mistake in a cell, click on that cell with middle mouse button to clear it. With two-buttons mouse interface and no middle button available, click both right and left buttons simultaneosly to clear the cell.

You may also hold down the mouse button and drag the mouse to fill several cells at once as you go.

While you are solving, you may want to mark out the numbers in the clues that you are certain about. To do so, click a number with left mouse button. The number will be crossed by a line. To clear the line from a number, click it with right mouse button.

After you complete an entire row or column, its clues will be highlighted. After you complete an entire row and also an entire column, the cells where they both intersect will be highlighted. In other words, if a cell is in a row and a column that are both complete, it is highlighted. The application does not actually check by now, whether the completion is correct. Such feature about checking the row is awaited in the future.


3. Might-be values

While you are solving the griddler, you may need to make temporary notes within the griddler. Do not use a pencil on you screen, please, you may damage your hardware. Hold down the Shift key instead and use your mouse as you do while solving the griddler. Instead of standard boxes and spaces, special might-be boxes and spaces are placed into cells. Those might-be values are not taken as a part of the solution, are drawn in a different color and in a different shape. This way you may easy your logic and see what would happen if.. This is called a level 1 recursion and is necessary for more difficult griddlers.

To clear all might-be values at once, click the Clear might-be button.


3. Undo, Redo

There are Undo and Redo buttons to help you make steps backward after discovering a mistake. The undo buffer is not saved into a grid-file by now, therefore you may go back only up to the step, where you have started. There is a possibility that this saving will be available in the future as it may be quite useful, but not yet.


4. Auto-solving

This application is a good solving workspace. I hope you have had a lot of fun with all the features that should have helped you. Anyway, the application is more about  the auto-solving.

To find one single step in the solving process, click the Find new piece of the solution button. The application will search for a next step and then fill several cells with its values. The cells will be highlighted for you to see where the auto-solver added what values. You do not need to recolor them by mouse. The highlighting will be forgoten upon next search anyway.

Even this application is not able to solve everything. If no available step is found, a message is displayed about the failure. However, that does not mean the griddler is unsolvable. You will have to help the application on your own to find another step. If you discover one, please, send me the partially solved griddler, highlight the next step (e.g. with might-be values), so I may work on that.. Thanks.

If you have a mistake in your partial solution, the search will work with your partial picture, thus working with your mistake. This may (and probably will) lead to making more mistakes and the search does not have to find out about it! It may become clear only after few another steps. You will be warned then about it, but the application will not be able to tell you, where the mistake is as it always work only with the clues and picture you actually see. Even if you have loaded a fully solved griddler and clered the picture just a while ago, the search does not possess any ability to cheat. All the steps the search finds and performs are also available to you, if you have the logic.

There is a possibility that a griddler has multiple solutions. While using the auto-solver, it may find out about that and will ask you which one to use. This is quite tricksy, because you will not see what it has actually found. There would be no use of that by now anyway. Therefore, you will have to pick one, "the first one" or "the second one". Hope you are lucky..

To see the entire solving process as one nice animation, click the Find all pieces of the solution. The search will subsequently find all the available steps of the solution. Nice to watch.. :)

If you are bored to watch step after step animation, click the Run full-pass iteration button to start a single full-pass search. The full-pass search means that all rows, columns and cells are scaned, one by one, for any available steps. All currently available steps are found at once.

To see an animation of all full-pass scans, click the Run all full-pass iterations button. All full-pass searches will be done subsequently. Also nice to watch but not always slow enough.. :)

If you want to solve the griddler and the animation does not bother you, click the Realtime, man! Realtime! button. The search will not be interrupted between the steps to display any results. It will stop only if the entire picture is solved; there are no available steps; or multiple solutions are found.

While searching for a solution, the griddler may be quite difficult and you computer not fast enough, click the Stop! button to interrupt a search. All already found values will not be forgotten, but the application will become usable again.


5. Editor

The application is also able to simulate a simple editor for griddlers. Check the Switch to editor mode checkbox to make the application behave as an editor.

While in editor mode, click with left mouse button in the clues area to add and increase clue numbers or click with right mouse button to decrease and delete clue numbers. Hold down mouse button and drag to increase or decrease clue numbers more flexibly.

If you are an artist and have a picture drawn already, you may click the Regenerate numbers from picture button. All actual clue numbers will be deleted and new will be calculated from the picture.


6. The format of a grid-file

The format of the grid-file where the griddlers may be saved is trying to be quite simple and editable also with a plain text editor. However, no chcecks are made upon load, whether the file is correct or not. If you edit a grid-file in a notepad, be sure you know the format well enough. If you screw the file, application may screw upon its loading. Sorry that I was quite lazy to prevent the application from crashing on bad files..

The first line contains a watermark and a file format version. Currently it is string "MK Version 3.0".

The second line is empty.

The third line contains sizes (width, height) of the griddler.

Fourth line is empty.

Note: All the next lines depend on the sizes a bit, therefore I am gonna stop numbering them.. :) This is where the file may probably end, if it has no clues and no pictures. Well, why not?

Next few lines contain the picture. Each line represents one row and consist of columns. Each column consists of a space and a cell value. The cell value is one of these: a hash "#" for a box, a dot "." for a space, a letter o "o" for a might-be box, a comma "," for a might-be space and a question mark "?" for an undecided cell.

Any other values are taken as undecided cells, however, this may change in the future, so stick with the question marks for your own good.

Lines does not have to contain all the columns. If a line is shorter, all the remaining columns are taken as undecided cells.

Note: This is where the file may end, if it has no clues. If you have drawn a picture in a text file, end the file here, load it into the application and let it calculate the clues.

Next few lines contain the clues for columns. The lines represents columns from left to right and numbers on them are ordered from bottom to top as they should appear in the clues. Use a negative number to indicate, that the clue number has a mark (crosing line over the number - see chapter Solving the griddler above).

Note: This is where the file may end, if it has no row clues. Well, why not?

Next few lines contain the clues for rows. The lines represents rows from top to bottom and numbers on them are ordered from right to left as they should appear in the clues. Use a negative number to indicate, that the clue number has a mark.

The rest of the file is not ever loaded, add any comments, stegano, or anything you want. Note: If the file is ever overwritten by the application, any such text will be lost, of course.
