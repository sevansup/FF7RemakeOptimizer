# FF7RemakeOptimizer
Optimizations for FF7 Remake on PC or Steam Deck. These are based off of the Ascendio mod for Hogwarts Legacy and likely will work with many other Unreal Engine 4 games. So far I can confirm this makes a massive difference in both FF7 Remake and Hogwarts on both PC and Steam Deck.

First you will need to have FFVIIHook installed and working. **If you are on Steam Deck, you need to rename the .dll file from FFVIIHook to .dxgi.dll** and place it in the proper in-game folder, otherwise it will cause conflicts with the Deck's controls. If on Windows, leave the .dll file named as is.
Place it in the game's directory under:

_FINAL FANTASY VII REMAKE\End\Binaries\Win64\_

Also, if you are on Steam Deck, you need to do one more thing **(ignore this part for Windows)**. You need to add this to the game's launch options in Steam:

_WINEDLLOVERRIDES='dxgi.dll=n,b' %command% -d3d11_

It should be located next to ff7remake_.exe (yes, the one with the _).

Then, download this [Engine.ini](https://raw.githubusercontent.com/sevansup/FF7RemakeOptimizer/main/Engine.ini) (right click > save as) and place it in the game's local data folder, which in this case is:

_%USERPROFILE%\Documents\My Games\FINAL FANTASY VII REMAKE\Saved\Config\WindowsNoEditor\_

If you don't have these directories, create them.

Open the .ini in a text editor like notepad and change the resolution on the first line to match your screen's resolution. If you're using the Steam Deck, you can leave as is because by default I have it set to 1280x800.

Enjoy! The game should feel much smoother and look sharper too, as this disables the game's glitchy dynamic resolution. If you're using any other performance mods for the game, disable them in case something conflicts with this method.
