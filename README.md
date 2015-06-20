# NITF_WalkingZeds_DayzEpoch
Walking zombies scripts

These are script files from dayz_code that have been altered to affect all zombie spawns to make them walk.
I have packed them into one folder and created an ini file to load them all. This way only one edit needs to be made to the init.sqf file to install. The zombie ini file does override a few lines from compiles.sqf. So if you have any zombie altering scripts running now that load from a custom compiles.sqf file. only one set will load properly. A murge will be needed if so, contact me if you need help murging with a custom zombie script.

Install - Easy

1. Copy the walkingzeds folder to the root of your mission.pbo

2. Open your init.sqf. "also in the root of your mission.pbo."

        Find    call compile preprocessFileLineNumbers "server_traders.sqf";		//Compile trader configs

ADD, Right under it
    
        call compile preprocessFileLineNumbers "walkingzeds\wdzini.sqf";    //NITF Walking Zombie Script

Repack and run. All zombies should walk.

I pieced this together from a handfull of differnt forums a while back for the last server i ran. So i am not sure who to give credit to. each file edit was listed under a differnt forum. It seemed no one had pieced together all the required files to alter every form of zombie spawn.
