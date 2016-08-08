# Java worm game

Classical worm game written in Java Swing using NetBeans IDE 8.1.

You should turn worm in purpose to eat apple. Every apple makes worm bigger for one piece and makes speed faster.

## Instructions:
You can adjust only field and figures sizes in the lines:

WormGame game = new WormGame(20, 20);

UserInterface ui = new UserInterface(game, 20);

## Description of packages and classes:

### 1. wormgame - contains main class and enum class
* main.java - contains main game parameters
WormGame game = new WormGame(20, 20);// constructs game with field width and height 20 and 20
UserInterface ui = new UserInterface(game, 20);// multiplication parameter for the side length of the field
* Direction.java - enum class for directions

### 2. worgame.domain - contains information about game creatures
* Piece.java - class that will be used to create worm.
* Apple.java - extends Piece
* Worm.java - contains of several pieces in ArrayList

### 3. worgame.game - contains game logic
* WormGame.java - contains worm, apple and actionlistener

### 4. wormgame.gui - graphical user interface
* UserInterface.java - main class for graphical interface, stores jframe, wormgame, drawingboard
* DrawingBoard.java - draws game creatures, repaint board according to update() method of Updatable interface
* KeyboardListener - listenes to keyPressed() method, changes the direction of the warm
* Updatable - interface for repainting the board
