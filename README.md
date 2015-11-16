# Tic-Tac-Toe Game
<img src="https://cloud.githubusercontent.com/assets/11559575/11175797/1034bdcc-8beb-11e5-8de6-4deb38a9d0c3.png"></img>
<hr>
RULES OF THE GAME:
It is randomly determined who goes first
When an empty square is clicked, it is recorded as a play for whoever's turn it currently is
When a filled square is clicked, nothing happens
We need to check for a winner after every play
When a winner is determined, the game halts, and the winner is announced
When the game reaches a stalemate, the game halts, and the stalemate is announced

# Tic-Tac-Toe Game Challenge: 
(About the Challenge)
LEARN Bootcamp Week 3: Create a Tic Tac Toe game with the knowledge you have learned using HTML/ CSS and JavaScript/ jQuery. Below is an outline for one possible solution that will get you started.

HTML
Create a grid for the Tic Tac Toe game that is 3 X 3
Using HTML you can create a table with a class=" grid'. Be sure to give it a height and width that will make it square
Within the table create 3 table rows < tr>
Within each table row create 3 table data cells < td>
Give each < td> a 'class'.
Give each < td> a unique ID as 'field1' through 'field9'. We will use the ID to identify each cell in later steps

CSS
Add CSS file to make the squares stand out and be easily clickable
Make the background be black
Make the < td> to be white
Get images of an "X" and "O" and make them accessible when you click
Give the < td> a fixed height and width
Give the table class a height and width
That gets our board setup, but nothing happens yet when we click on the squares because we haven't used Javascript yet to create the interactions. We will need to put our scripts and links to our Javascript, styles and JQuery so don't forget to put those in the head section of the html.

Javascript/JQuery
We will need to put our scripts and links to our Javascript, styles and JQuery so don't forget to put those in the head section of the html.
We are going create the functionality of the Tic Tac Toe through an Agile development model. This will allow us to create small chunks of code that can than be tested immediately before moving on to the next task.
On to the JavaScript file you are going to need to create your functionality. This will be the part that will test your creativity.

Task 1
Story: As a user, I can put 'X' anywhere on the board.
Task: Create a function that is run when a user clicks on a square and
changes the square to 'X'.

Task 2
Story: As a user, I can only put 'X' on the board where there are no markings already.
Task: Change the function so that If the square is already filled, do nothing; otherwise, fill in square.

Task 3
Story: As two users, we can alternate between putting 'X' and 'O's on the board; starting with 'X'.
Task: Create a variable to hold the current player's marker, use it in the function created above, and change it after each move.
Task 4
Story: As two users, we can only place markings where there are no markings already so that we cannot override our own or the opponents markings.
Task: See Task 2.

Task 5
Story: As two users alternating between putting markings on the board, the computer will inform us when there are no more empty positions and the game is over.

Task: Create a function that checks the board for empty positions and return true if there are empty position; then add to the function above a check of the board and an alert if the the board is full.

Task 6
Story: As two users, playing the game, when board is full, the computer
will tell us who won 'X' or 'O' or if the game ended in a stalemate.

Task: 
Setup a data structure for winning combinations.
This needs to list all possible winning cell combinations
If we think about our table as being labeled 1,2,3 across the first row, and 4,5,6 for the middle, with 7,8,9 in the bottom, 1,5,9 and 3,5,7 diagonally
Create function that checks for a winner.
Iterate over all possible winning cell combinations to see if any are completely filled in with either X or O

Task 7
Story: As two users, playing the game, as soon as a player won the computer
will tell us who won 'X' or 'O'.
Task: Reuse functions from task 6.

Extra Credit Task n:
Story: As two users, before the game starts, the computer asks for each player's name so that the computer can prompt the users with their name when it's their turn.
Task n+1:
Story: As two users, before the game starts, the computer asks for each player's name so that the computer can name the winner at the end of the game. 
Task n+2:
Story: As two users, after a game, the computer asks if you want to play again, and if so resets the board so that the users do not need to enter their names again.

Task n+3:
Story: Most of the time players will play several games of Tic Tac Toe in a row. They will want to keep track of the number of times 'X' won, and the number of times 'O' won. They will also start the next game with the winner of the last game going first. For extra extra credit, we are going to refactor our working Tic Tac Toe Query game to handle these multiple game behaviors.

New rules determining multiple game sessions.

First game continues to start with random X or O turn
When the new game button is pressed, the win is recorded for X or O, and the board resets
Whoever won the last game will go first in the new game

