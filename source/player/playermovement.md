## playermovement.cpp

This file is used to handle pressing WASD to move player
- Refrenced in player.h

#### player::Movement()
- This function handles WASD keys
- - W moves up
- - A moves left
- - S moves down
- - D moves right
1. Detects if W/A/S/D key pressed
2. Checks if player will go off bounds of map
3. Checks if there is block on place where will player go
4. If there is no block there then remove current player from map (prevent leaving ghost player) and update player position