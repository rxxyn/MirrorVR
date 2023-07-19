# MirrorVR
![MirrorVRWideTransparent](https://github.com/rxxyn/MirrorVR/assets/113850083/4ab6122f-45bb-4550-ac9c-d39bc4b7bc71)


### Mirror VR is a Unity plugin that uses the [Epic Online Services transport](https://github.com/FakeByte/EpicOnlineTransport) by FakeByte with [Mirror](https://mirror-networking.gitbook.io/docs/) to create an easy, free, and beginner-friendly experience for multiplayer VR games.

## NOTICE: THIS HAS NO RELEVANCE WITH FCHB1239 OR PHOTONVR. MIRROR VR HAS ABSOLUTELY NOTHING TO DO WITH IT.

### NOTE: This plugin will be in development for quite a bit. I am aiming to fine tune this as much as possible.
#### For using Mirror VR with Android, you will need to follow a very, VERY, exact tutorial.
#### Check back later for more information.

&nbsp;

# Syntax example

To use MirrorVR, lets use it!
```cs
using MirrorVR;
```
Setting Names
```cs
string name;
MirrorVRManager.SetUsername(Name);
```
Setting Colors
```cs
Color colour;
MirrorVRManager.SetColour(colour);
```
Finding lobbies
```cs

//finding lobbies without lobby search parameters

uint maxlobbyResults = 5;
MirrorVRManager.FindLobbies(maxlobbyResults);

//finding lobbies with lobby search parameters

uint maxlobbyResults = 10;
LobbySearchSetParameterOptions[] lobbySearchSetParameterOptions = new();

MirrorVRManager.FindLobbies(maxLobbyResults, lobbySearchSetParameterOptions);
```

Creating lobbies
```cs
//the first parameter is a boolean,
//if you want to have a custom name for your lobby, enter true.
//if not, enter false and don't include a string for the second parameter.

string lobbyName;
lobbyName = "mirrorvr";

//this is a lobby with a custom name.
MirrorVRManager.CreateLobby(true, lobbyName);

//this is a lobby with a randomly generated name. (not custom)
MirrorVRManager.CreateLobby(false);
```
&nbsp;

# DOCUMENTATION

#### For full documentation on Mirror VR, navigate to the top of this repo and press Wiki.
#### If you would just like a shortcut, click [here](https://github.com/rxxyn/MirrorVR/wiki)

&nbsp;

# PLANNED

-Full Android documentation (Iykyk)<br />
-Relativly easy implementation  <br />
-Host migration <br />
-Synced cosmetics<br />
-Synced colors<br />
-Synced names<br />
-Easy presets for grabbables<br />


&nbsp;
# CREDITS

JokerJosh - 2nd Developer <br />

Mirror and Epic Games - servers and backbone <br />

FakeByte - the relay, (the 2nd backbone) <br />
