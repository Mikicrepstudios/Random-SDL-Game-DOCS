## playercontrols.cpp

This file is used to handle mouse click functions
- Refrenced in mouse.h

#### mouse::Event()
- This function handles placing blocks and quick color picker

1. If left click is pressed then place block on current mouse position
2. If right click is pressed then destroy block on current mouse position
3. If color picker is active and left click is pressed then get color from current mouse position

#### mouse::Overlay()
- This function handles drawing of mouse highlight

1. If background color is not white then draw white highlight on current mouse position
2. If background color is white then draw black highlight on current mouse position
3. If camera highlighting is enabled and background color is not light red then draw light red highlight on current mouse position
4. If camera highlighting is enabled and background color is light red then draw dark red highlight on current mouse position

- - SDL_Rect mouseRect = {curHoverX * cam.scale, curHoverY * cam.scale, cam.scale, cam.scale} is used to calculate on which block is mouse currently hovering