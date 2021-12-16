# Josh-Checkers-Game

# Description:

Checkers, also called draughts, board game, one of the world’s oldest games. Checkers is played by two persons who oppose each other across a board of 64 light and dark squares, the same as a chessboard. The 24 playing pieces are disk-shaped and of contrasting colours. At the start of the game, each contestant has 12 pieces arranged on the board. While the actual playing is always done on the dark squares, the board is often shown in reverse for clarity.

- [Source](https://www.britannica.com/topic/checkers)

# About Checkers Game:

Today’s game of checkers developed around the start of the 12th century. A Frenchman came up with the idea of playing checkers on a chess board. At that time, the game was called “Fierges” or “Ferses.” With a new board design and new rules set, the game made its way to England and the Americas.

Today, most English-speaking countries use a 64-space checker board. This is known as the short king board version. However, much of Europe and Asia use a checker board with 100 spaces. This is called the long king version. Some people in Canada even use a board with 144 spaces!

Checkers remains a popular game around the world today. For many children, it’s the first game they learn how to play. Teachers have long known that the simple game of checkers can provide significant training in thought and logic. Of course, it also keeps players occupied with fun competition.

- [Source](https://wonderopolis.org/wonder/Which-Came-First:-Checkers-or-Chess)

# Reviews

<IMAGE>

# Technologies Used:

JavaScript, HTML, CSS...

# Instructions:

1. Take Control of the Center
   Beginners often place their checkers on the edge of the board. This seems like a reasonable strategy, because your pieces on the edge cannot be captured.
   But as it turns out, pushing your checkers to the edges is a mistake.
   Try to form a pyramid shape with your pieces.
2. Play offensive
   Because of the possibility of forced moves, your opponent can presents you with a capture you must take. Because of this, you cannot afford to sit back and fortify.
   You could be forced to jump your checkers into oblivion at any time and no defense that you build can stand up over time.
3. Play according to the strength of your position
   Attack only on the strong side and defend only with on the weak side.
4. Never move a piece without a notive
   If you wish to become a master player, you need to learn how to "plan" and not merely live from one move to the next.

5. Stick together when you advance
   A single checker advanced can easily be jumped and captured while a checker backed up by two more checkers is immune from capture.
   If you press forward with a few checkers then your advancing force will be much more powerful.

6. Crown your pieces to kings
   A kinged piece is incredibly powerful. The player who kings more checkers will usually win.
   While capturing opposing checkers is generally a good thing, your biggest concern should always be kinging your own checkers.
   Sacrifice a checker if needed
   You should be willing to trade a capture for a capture when it advantages you.
   Use this to capture an opponent's advanced checker or to clear out some of his base row checkers.

7. Sacrificing a checker to clear a path to be kinged is always worth it.

If you can trade one pieces for two, you made a good choice.

8. Trade pieces when you are ahead
   With only 12 pieces on the board for each player, it is quite possible that you may quickly end up with a 8-7 piece advantage and if you can trade four pieces, you suddenly have a 4-3 advantage which is a tremendous amount of power.

9. Move your home row checkers only when you need them
   Your opponent cannot get any kinged checkers without advancing into one of your four home spaces.
   Keeping these spaces occupied guarantees that your opponent will get no kings until your checkers move. 10. Attack you opponents "Double Corner"
   It is preferable to break through the Double Corner side because a piece that crowns can usually emerge there more easily than one which reaches the Single Corner.

10. Be aware for kings in the endgame
    Once only a few pieces are left on the board, the path to kingship will be open. Don't trade pieces blindly if it means that your opponent will be closer than you to get a king.

11. Win by blocking
    If you cannot move a piece on your turn, you lose.
    If you can block in your opponent's checkers, you will win.

12. Play against better players
    While winning is fun, you can't learn much by playing against weaker players.

- [Source](https://www.ultraboardgames.com/checkers/tips.php)

# Wireframe:

![Alt text](https://git.generalassemb.ly/josh-vn/Josh-Checkers-Game/blob/master/img/wireframe.png)

# Pseudocode:

1. Define required constants

- define square that checker can go to: validSquare
-

2. Define required variables used to track the state of the game

- define Current player: Red / Black
- define game active or not: True / False
- define winning player: ''
- define possible move 1, 2, 3, 4(king)
- define count down how much checkers each person has

3. Handle event listener

- Player clicking a square

  - Validate if the square have the checker (red & black)
  - Validate their checker (black / red)
  - Check if it have any possible move
  - Show / Highlight the possible square to move
  - Click again to undo Validation
  - Or click another square and start again

- Player clicking a square to make move

  - Delete the checker in original square
  - Place the checker in the possible move chosen
  - If go pass other's player checker -> delete their checker
  - Set count down how many checker each player has
  - Check again for any other possible move
  - If yes:
    - Auto place the checker in the possible move
    - delete other's player checker
    - Set count down how many checker each player has
  - If checker reach last row from each side:
    - Delete the checker that square
    - Place the KING checker that square
  - Switch to other player turn

- player clicking quit/replay button
  - Reset active game status
  - Reset player move/turn
  - Remove all player's checkers
  - Place all player's checkers at starting point
  - Reset countdown

4. Function to handle event

- Render function

  - Reset active game status
  - Reset player move/turn
  - Remove all player's checkers
  - Place all player's checkers at starting point
  - Reset countdown

- Checker Selection Function

  - Validate if the square have the checker (red & black)
  - Validate player checker turn (black / red)
  - Click again to undo Validation
  - Or click another square and start again

- Check Possible Move Function

- Handle Move Selection
