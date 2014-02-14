flashcard
=========

Prepare plain-text flashcards and view them on the terminal

Usage
=====

    usage: flashcard: [-h] [-a] [-s] file1 file2
           -h    Show this help
           -s    Shuffle the deck
           -a    Alternate the first side of the card to be shown, randomly

where `file1` and `file2` must consist of equal number of lines, line 1 of `file1` is the front of the card, line 1 of `file2` is the rear of the card, etc.

After a card is shown, type your guess and press enter. The other side of the card will be shown afterwards.

TODO
====

* Be able to rate how well you remember an option
* Make a tool for generating flashcards easily
