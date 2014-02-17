# flashcard

Prepare plain-text flashcards and view them on the terminal

![flashcard screenshot](http://bugsofberk.net/assets/flashcard.png)

# New features

* You can now write a file in dictionary format, much like the Python dictionary syntax.

# Usage

    usage: flashcard: [-h] [-a] [-s] file1 [file2]
               -h    Show this help
               -s    Shuffle the deck
               -a    Alternate the first side of the card to be shown, randomly
    
    	   If file2 is omitted, it is presumed that the file is in dictionary format.

If two files are specified, the two files must contain the same number of lines. See the examples for an idea of how the flashcard files should look like.

After a card is shown, type your guess and press enter. The other side of the card will be shown afterwards.


## Examples directory
An example deck (beginner Swedish vocabulary) can be found at the `example` directory. It has been fetched from [this wonderful Online Swedish course by Björn Engdahl.](http://www.onlineswedish.com/main.php)

The `two-files` subdirectory contains the examples in old format. The `dictionary` subdirectory contains the examples in the new format, which allows generating flashcards from a single file.

## mkdeck helper script
mkdeck can be used with flashcard to generate a dictionary formatted file from two files (old format).

        usage: mkdeck: [-o output] [-e] file1 file2
               -o    Specify the output file, stdout by default
               -e    Define the Python source encoding (PEP 0263), utf-8 by default
               -h    Show this help

# Known Issues

* Files in the dictionary format are not read into the program in the correct order of entries.
* mkdeck doesn't tabulate the output very well.

# TODO

* Be able to rate how well you remember an option
