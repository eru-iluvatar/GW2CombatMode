GW2CombatMode
=============

![Screen Shot](screenshot.jpg)

This is a C# .NET tool based on the Guild Wars 2 Combat Mode MOD by Michael Puckett & Jayce. It's currently in BETA.

Why make another version?
=========================

There's a couple of reasons why I made another tool altogether:

Configurable Settings
---------------------
This tool has a UI to configure all settings, so you don't need to dig into code to change options. 
I'm also planning to enable several settings, so you can have separate ones for each of your characters.

More Options
------------
There are several additional options you can configure:

-Shut down the tool when you close Guild Wars 2
-Start the tool minimized (currently to the task bar, working on System Tray)
-Vertical Offset for the cross-hair overlay
-More control over cross-hair display in/out of combat mode
-Auto-enable combat mode when using a skill key
-Auto-switch combat mode when switching weapons
-Auto-disable combat mode when chatting or opening UI windows (e.g. inventory, etc.)
-Toggle tool visibility, so it's as close as possible to a GW2 UI window

Mouse Trap
----------
These MODs (both the original and mine) require you to run Guild Wars 2 in Windowed Mode. If you have a dual screen setup, like me, you know what that means: the mouse is not "trapped" in your game screen but can move off to your second screen desktop while you're gaming. 
So I added an optional mouse trap that locks the mouse on the primary screen in Windowed Mode.  


Runtime
-------
The original tool is written in AHK (AutoHotKey), which is an interpreter, not a compiler. 
This means every time the tool executes a line of code in the script, it is re-interpreted. 
For this reason, the original tool is kind of CPU hungry (it typically consumes between 5 & 10% of my CPU).

.NET is a JIT (Just-In-Time) compiler, which means the code is compiled ONCE and then executed natively - it is therefore much faster and requires much less CPU (the .NET version usually indicated between 0 and 1% of CPU usage in Task Manager).    

 