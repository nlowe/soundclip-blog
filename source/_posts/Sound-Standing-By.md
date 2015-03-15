title: Sound Standing By
date: 2015-03-15 15:34:43
tags:
---

Well, I think I'm ready. I've made a decent amount of bug fixes and added a few critical features that I think I'll need for this production. We open in two weeks, so here we go!

### Changes since last update:

* Consecutive clicks of the panic button now perform a hard-stop instead of infinitely fading out
* Transport Context Menus show for playing cues even when the workspace is locked
* Better detection of audio file duration
* Validation of audio files (does the OS have the needed plugins for playback)
* Fix a bug where new projects could not be saved
* Fix a bug where cues would fade out a few seconds after starting if a panic was previously initiated
* Support replaygain tags in audio files
* Basic transport controls and cue notes viewer

<!-- more -->

![](gui.png)

Unless anything else comes up, I'll cut `alpha2` after practice tomorrow.
