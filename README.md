# Elevens 8

Follow the instructions provided for Activity 8 in the student lab guide. This is more of an exploratory lab, so you will not need to copy any of your previous code into the repo. Answer the questions from the Student Guide in this document and ensure that you save and push the repo. You have one week to complete this lab.

1. Discuss the similarities and differences between *Elevens*, *Thirteens*, and *Tens*.

    * All three have an aspect of the game where summation to 11/10/13 with a standard card deck is important. While the whole deck is used, each game varies in the aspired sum, and so cards greater than that number have their own rules depending on each game. In 11s and 10s, combining facecards is a notable portion of play. They each have different odds of winning as well, with 13 having a one in two times, 11 having a one in four times, and 10 having a one in eight times.

2. As discussed previously, all of the instance variables are declared in the `Board` class. But it is the `ElevensBoard` class that “knows” the board size, and the ranks, suits, and point values of the cards in the deck. How do the `Board` instance variables get initialized with the `ElevensBoard` values? What is the exact mechanism?

    * Board is a superclass meant to define the deck of each game. To initialize the instance variables it uses polymorphism to call the ElevensBoard object.


3. Now examine the files `Board.java` and `ElevensBoard.java`, found in this repository. Identify the `abstract` methods in `Board.java`. See how these methods are implemented in `ElevensBoard`. Do they cover all the differences between *Elevens*, *Thirteens*, and *Tens* as discussed in question 1? Why or why not?

    * Abstract methods include board, isLegal, and anotherPlayIsPossible. Other methods seem to cover all the differences between games. In isLegal and anotherPlayIsPossible the methods are generic enough to implement individually to each game, and the board method takes in parameters that would change depending on each game.
