Proposed Project: Slot Machine
Idea: an amount of money ($10.00) will be inserted in the code and then you run the code to start the machine. The LEDs will show how much money you have and then when you press a button, the 5 leftmost LEDs jumble through an array of different symbols and eventually stop on random ones. If three or more match then a specific multiplier is added and is displayed on the farthest right. After that the amount that the player has with the multiplier will be displayed. If nothing hits, the player will lose $2. Multipliers will be higher depending on how many symbols match. The second button on the board will signify ending the game and taking winnings


The combinational logic will include code needed to check whether symbols match, determining multiplier amounts, calculating winnings and converting binary to display.
The sequential logic includes storing the random symbols after a spin, calculating player balance, keeping track of what state the game is in (spin, displaying results, ready, etc.), and using a background randomizing system that will determine the random symbols that will appear after rolling


The final submission should showcase the input phase where $10 is inputted in the code and the amount is shown on the board. Then when button 0 is pressed the 5 leftmost LEDs should spin random symbols and then show a multiplier on the side. It should then switch after a second to the new total that the player has. It should be run until all multiplier combination cases are shown (most likely will have to edit video due to randomability). New values after spinning should be accurate and the game should finish when either player loses all money or player presses button 1. 

TA Feedback:
Fun project and a good size for two people. A few things to sort out: the symbols will be on the 7-segment displays (not the LEDs), so pick symbols they can actually show. An LFSR works well for the random part. Also make it clear what the multiplier applies to (for example, a $2 bet), so the new balance is easy to check. Since getting every match case by chance could take forever, add a switch “test mode” that forces specific results for the demo. Please include who did what in the final report.

Rubric (out of 10):
Starting balance of $10 shown on the displays - 1
Button 0 starts a spin, symbols cycle and then stop - 2
Random symbols generated (LFSR or similar) - 1.5
Match checking with the correct multiplier shown - 2
Balance updated correctly after a win or a loss - 2
Game ends on button 1 or when the balance hits 0 - 1
Test mode to show all multiplier cases - 0.5
