This is a silly hack of https://github.com/snesrev/sm/ , to make the window move around your desktop as the camera moves, like it's a spotlight on the game world.

I slapped this together because I couldn't sleep after having the idea.  I have no idea whether it actually keeps working correctly beyond the first couple areas of the game.

There's currently no logic at all for door transitions, it just naively moves as far as it can towards your new position, though in practice that works surprisingly well in most rooms that I've seen, once you're past Ceres Station?  Feel free to drag the window around your desktop to give it room to wander in as needed.

One known issue is, the window's movement is weirdly twitchy if your monitor's refresh rate is not 60 Hz.  No idea why, sorry.

Part of me is tempted to add a second window behind the gameplay window, displaying a full-game screenshot map that pans around to be in sync with the main window, but that would mean manually assigning coordinates to every room in the game, and I'm not sure if I can be bothered...    tempting, though...


Original readme follows:

# sm

Our discord server is: https://discord.gg/AJJbJAzNNJ

Early version. It has bugs and the code is messy.

For building instructions, see: https://github.com/snesrev/sm/blob/main/BUILDING.md

Put sm.smc (sha1 hash da957f0d63d14cb441d215462904c4fa8519c613) in the root folder. When running, it will run both versions and compare frame by frame. If it detects a mismatch, it saves a snapshot in saves/ and displays a counter on screen counting down from 300.

