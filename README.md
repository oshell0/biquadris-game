# Biquadris Game

Biquadris is a 2-player, turn-based falling-block puzzle game inspired by Tetris but with additional mechanics, levels, and special effects.

Final project for CS246 - Object Oriented Programming.

#### Features
- Classic falling-block mechanics
- Multiple levels (0–4), each with unique block generation behavior
- Special effects triggered by opponent actions:
    - BlindEffect
    - HeavyEffect
    - ForceEffect
- Two independent boards (Player 1 & Player 2)
- Turn-based gameplay
- Score calculation and row clearing
- Random or deterministic block generation
- Rotation, movement, and drop system
- Text and X11 graphical display
- Score and all time high score tracking

#### Tech Stack
- C++20 (Modules TS)
- X11 for graphics
- GCC 15/GCC 14
- Makefile build system

## Gameplay 

### How to Play
- On your turn, control the falling block by moving left or right, rotating, or dropping.
- Place blocks to complete full horizontal rows, full rows get cleared, cleared rows earn points and clearing an entire block gains extra points.
- Clearing multiple rows at once allows you to apply challenge effects to your opponent, making their next turns harder.
- Players can level up and level down to change their difficulty level.
- After placing a block, your turn ends and the other player goes next.
- Keep stacking efficiently to avoid reaching the top of the board.
- The game ends when a player can’t place their next block.
- The remaining player wins.

### Commands
Players interact with the game through textual commands:
- Movement (`left`, `right`, `down`)
- Rotation (`clockwise`, `counterclockwise`)
- Dropping (`drop`)
- Level manipulation (`levelup`, `leveldown`)
- Special actions (`restart`, `random`,`sequence file`)
