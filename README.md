# Person and Bunny Game - C# 🐇

A console-based 2D grid survival game written in C#. The player (`P`) must escape a dangerous lair before rapidly multiplying mutant bunnies (`B`) spread across the board.

## 🎮 How It Works
* **Grid Setup:** Reads matrix dimensions (`rows` and `cols`) and the initial board layout (`P` = Player, `B` = Bunny, `.` = Empty cell).
* **Movement:** The player moves using a sequence of commands (`L` = Left, `R` = Right, `U` = Up, `D` = Down).
* **Bunny Spread:** After every player move, each existing bunny spreads to all four adjacent cells (up, down, left, right).
* **Win / Loss Conditions:**
  * **Win:** The player successfully steps outside the boundaries of the grid.
  * **Lose:** The player steps onto a bunny or gets overtaken by spreading bunnies.

## 💻 Example Input & Output

**Input:**
```text
5 6
.....P
......
...B..
......
......
ULDDDR
