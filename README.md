#  <img src="https://raw.githubusercontent.com/PMMP-To-Stead/Steadfast2/master/steadmplogo.png" alt="SteadMP logo" title="Gofight" align="center" height="320" />
# SteadMP Minecraft PE Server Software

## Introduction

Steadfast2 is a project for backporting new Minecraft: Pocket Edition changes to older Pocketmine versions for better stability and performance, while retaining as many features from the new versions as possible. It's currently in production on Lifeboat Survival Games' main servers.

SteadMP is a project created by me for adding some of the latest PMMP API codes and features to Steadfast2 according to my server needs.

SteadMP is a fork of Steadfast2 and spoon of PMMP and other Pocketmine related softwares.

## Already added features
- [x] Support for pocketmine's FormAPI plugin
- [x] Support for MyStats Scoreboard API from VixikHD(You just need to change packet usages to steadfast's one)

## Known bugs

- Players don't fall out of the world naturally, you'll want to handle PlayerMoveEvent as needed to kill them.

## Installation

### Installing On Linux/MacOS

To install SteadMP on Linux OS/MAC OS please follow the instructions below.

1)  `git clone git@github.com:Hydreon/Steadfast2.git` or `https://github.com/PMMP-To-Stead/SteadMP.git` in directory of your choosing. Or download and extract the zip into the directory of your choosing. 

2) Navigate to `SteadMP` directory via command line

3) Run command `./installer` If successful this will create a `bin` directory with a special Php7 build in it and a `start.sh` shell script
    
4) Running `./start` for the first time will take through the setup wizard where and create the 2 main config files for your server `pocket####mine.yml` and `server.properties`    

  *Linux VM Notes:* 
        
   - If using Vagrant have a config of `config.vm.network "public_network"` in the `Vagrantfile` should make your server discoverable from LAN. 

### Installing on Windows

SteadMP is not the best suited for running on Windows and another fork of Pocketmine would be better for that. But don't worry SteadMP will still run on Windows OS with some lack of performance,

To install SteadMP on Windows OS please follow the instructions below.

1) To install SteadMP on windows OS, first you need to download the PocketMine PHP7 installer -> [from here](https://github.com/NotPocketMine/Windows-PocketMine-MP/) "Always take caution when downloading binaries off the internet" :)

2) Next, you need to run the PocketMine installer then follow the instructions provide in the installer. 

3) Then you need to navigate to your user's documents file, and delete PocketMine-MP.phar.

4) Finally, you need to move SteadMP.phar into the directory above and run start.cmd.

We suggest a Linux VM in the meantime.  We also suggest using Vagrant and picking a Ubuntu box -> [from here](https://atlas.hashicorp.com/boxes/search?utf8=%E2%9C%93&sort=&provider=&q=ubuntu)
   
## Most Commonly Asked Questions

### Starting/Stopping Server On Windows

1) To start the server navigate to your user's documents file, and click start.cmd
2) To stop the server navigate to your user's documents file, and close the start.cmd windows

### Starting/Stopping Server On Linux/Mac

 1) To start the server open a terminal window in the server root directory and then run command `./start`.
 2) To stop the server type `stop` in the terminal of the running server. (or CTRL + C should work).  
 
## Creating the SteadMP.phar File

To build the SteadMP server phar file please follow the instructions below.

1) Download the SteadMP master from GitHub, then unzip the master then move the src folder into your server directory, then deleted the old .phar file if you still have it in the server directory. 

2) Download the [PocketMine DevTools Plugin](https://poggit.pmmp.io/p/DevTools/1.12.1) then move the plugin into your server directory plugins folder.

3) Start the server if you don't know how to start the server follow your Starting/Stopping Server instructions above.

4) Then run makeserver in the server terminal, then it will drop the phar file in its plugin directory.




