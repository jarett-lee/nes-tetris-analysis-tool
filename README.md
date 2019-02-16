# NES Tetris Analysis Tool

This tool is intended to help NES Tetris fans understand the game. In particular, players and commentators can identify when there's a run of bad pieces, but a casual fan watching a game without commentary wouldn't realize that was the case.

## Plan Forward

Currently, the plan is to make a personal use tool that reads the screen and displays visualizations in a separate window.

### Current Goal

1. Calculate possible piece placements given a board state
2. Read a board state from a video

### End Goal

* Components
  * Screen reader - pixels to Tetris state
  * Analyzer - Tetris state to statistics
  * Visualizations - statistics to display

* Screen Reader
  * Capture pixels
  * (Sample pixels)
  * Clean input

* Analyzer
  * Piece dependencies
    * A well 4 blocks deep is (usually) an I piece dependency since that's the only piece that can fit without causing
      a hole
  * Percentage of time a Tetris is possible
  * Average time to get an I piece after a Tetris is possible
  * Average time without an I piece and the Tetris well closed
  * Calculate the optimal sequence of future moves to make a Tetris
    * Did the player make the right move?
      * Keep in mind there's a lot of factors that can affect this including risk
  * The pieces that the current state can accommodate
  * The pieces that the current state can accommodate and into the future

* Visualizations

## Resources

* https://meatfighter.com/nintendotetrisai/
