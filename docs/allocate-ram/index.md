## Allocating More RAM
Modded Minecraft often needs to use more ram than Vanilla does to ensure it runs smoothly.  
If you're having performance issues, or your game crashes with an `OutOfMemoryException`, then you should try allocate more ram in your launcher settings.

#### What's the Best Amount of RAM?
It's a good idea to be conservative with the amount of ram you allocate. You want to assign enough to allow your game to load and run without the `OutOfMemoryException` crashes, but not so much that Java struggles to manage the memory (causing frame-stuttering/lag).

A good starting point for modded minecraft is 2GB.

#### Mojang Launcher
Follow the steps taken in the video to open the launch options for your modpack profile.  
Under 'JVM Args' modify the `-Xmx#G` value, changing the `#` to the number of Gigabytes you want to assign.
This will become the maximum amount of ram that the game can use.

<video src="mojang-jvm-args.mp4" width="560" height="350" controls preload></video>

#### Modpack Launcher
Open the launcher Options window and modify the 'Maximum memory' value.  
**Note - this value is in Megabytes, not Gigabytes.**  
There are 1024 Megabytes in 1 Gigabyte, so to allocate 2 Gigabytes of ram, enter a value of 2048.

<video src="launcher-jvm-args.mp4" width="560" height="350" controls preload></video>
<br>
<br>

##### Regarding the other settings:
- 'Minimum memory' - this should never be higher than the 'Maximum memory' value. 
- 'PermGen' - this has absolutely no effect when running the game with Java 8 or above, leave it alone, or set it to any value - it doesn't matter!
