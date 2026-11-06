# xr-game_eng-assignment-1-

## Guitar learning 
my idea is a guitar learning platform similar to slopsmith (now feedback). as i have been using rocksmith on my pc for years.
I will support the open format for song files so people can use already existing song tabs.
Using the hand tracking i can identify what fingers are being used etc and critique that. 

The goal is to teach the user to play the guitar by visually showing incoming notes and where to play them with feedback.
Dependancies:
* Godot 4 built-in OpenXR: it’s in core, nothing extra to install.
* godot_openxr_vendors (GodotVR): for Quest builds, passthrough, spatial anchors and hand tracking extensions.
* godot-xr-tools: menus, pointers, interaction. Optional, but it saves building song-select UI from scratch.
* Spatial anchors: let the player pin the note highway (or a virtual fretboard overlay) relative to where they sit or hold the guitar, and keep it there between sessions.
* gdext: for writing audio analysis most likely in rust with dependencies like cpal
