# botamusique
[Version Française ici](README.fr.md)

======

Botamusique is a mumble bot which goal is to allow users to listen music together with its audio output.
Predicted functionnalities will be the one you could expect from any classic music player.

Bot the can play :
- Radio url
- Youtube/Soundcloud URL (everything supported by youtube-dl)
- Local folder (disabled, I need to work on the web interface)

#### Web interface
* Disable * I need to work on it. Since I use this bot for radio, youtube/soundcloud and folder music, the web interace isn't ready.

You need to create a folder for all your music. Organize your music by subfolder.
The main folder need to be declare into the config (with a '/' at the end)

#### Installation
1. You need python 3 with opuslib and protobuf (look at the requirement of pymumble)
2. The Bot use ffmpeg, so you know what you have to do if ffmpeg aren't in your package manager. I personally use [this repository](http://repozytorium.mati75.eu/) on my raspberry.

commands (don't forget the sudo mode):
```
apt-get install python3-pip
apt-get install ffmpeg
git clone --recurse-submodules https://github.com/azlux/botamusique.git
cd ./botamusique
pip3 install -r requirements.txt
chmod +x ./mumbleBot.py
```

#### Starting the bot
./mumbleBot.py -s HOST -u BOTNAME -P PASSWORD -p PORT -c CHANNEL

The bot listen to the 8181 port so you should redirect to this one in you NAT configuration to let others peoples access the web interface. (DISABLED)


2.TODO list

### TODOLIST

#### Features
- [x] Next song
- [x] Randomizer
- [ ]Graphical interface

#### Commands with the interface (disabled)
- [x] list
- [x] play
- [x] playfolder
- [x] random

#### Commands by message to the bot
- [x] volume
- [x] next
- [x] stop
- [x] joinme
- [x] away
- [x] help

#### Web Interface (disabled for now)
- [x] Primary functions
- [ ] CSS
