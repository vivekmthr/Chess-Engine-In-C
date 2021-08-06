# Chess-Engine-In-C

**Introduction**
This repo contains my implementation of a Chess Engine. It is still in progress, and the game analysis functions are in the progress of being optimized and built.

**Design**

1. _Board Initialization_
  - The board is initialized as 16 different bit-boards. These are used to track the current position of each different piece. We use bit-boards as they are more space effective and increase effieciency significantly. 
2. _Move Generation_
   - We can create bitboards by using XOR and XAND operations like location of black pieces, location of white pieces so on. 
   - Using these extra boards along with bit shifts allows us to calculate the possible moves for each piece. 
   - Sliding move generation is a little bit more complex, and this is done using magic bitboards. 
3. _The AI_
  - The AI currently is very basic and uses a search tree with alpha beta pruning to find the best series of highest scoring moves depending on the opponent.

**
**Building**
Navigate to the alpha beta folder and runn Chess.c.
