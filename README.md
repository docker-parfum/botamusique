# botamusique

**Info:**

> This is a fork of the official repository (located [here](https://github.com/azlux/botamusique)).
We are working on various features for our own version of the bot. However, we will
regularly merge upstream changes and will also create pull requests to merge back our
features to the upstream repo at some point.

The remainder of this readme is from the original repo.
Note that the ToDo list at the end of the Readme is **outdated** and **not applicable** for this repository.

---

[Version Française ici](README.fr.md)

======

Botamusique is a mumble bot which goal is to allow users to listen music together with its audio output.
Predicted functionnalities will be the one you could expect from any classic music player.

1. Where to start

You need to create a folder for all your music. Organize your music by subfolder.
The main folder need to be declare into the config (with a '/' at the end)

#### Installation
1. You need python 3 with opuslib and protobuf (look at the requirement of pymumble)
2. The Bot use ffmpeg, so you know what you have to do if ffmpeg aren't in your package manager. I personally use [this repository](http://repozytorium.mati75.eu/) on my raspberry.

commands (don't forget the sudo mode):
```
apt-get install python3-pip
pip3 install opuslib
pip3 install protobuf
pip3 install flask
apt-get install ffmpeg
git clone --recurse-submodules https://github.com/azlux/botamusique.git
cd ./botamusique
chmod +x ./mumbleBot.py
```

#### Starting the bot
./mumbleBot.py -s HOST -u BOTNAME -P PASSWORD -p PORT -c CHANNEL

The bot listen to the 8181 port so you should redirect to this one in you NAT configuration to let others peoples access the web interface.


2.TODO list

### TODOLIST

#### Features
- [ ] Next song
- [ ] Previous song
- [x] Randomizer
- [ ] Looking for songs previously downloaded in a folder by users.

#### Commands with the interface
- [x] list
- [x] play
- [x] playfolder
- [x] random

#### Commands by message to the bot
- [x] volume
- [ ] skip
- [x] stop
- [x] joinme
- [x] away

#### Web Interface
- [x] Primary functions
- [ ] CSS

