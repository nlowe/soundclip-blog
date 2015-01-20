title: Let There Be Sound
date: 2015-01-20 06:52:26
tags:
---

SoundClip `master` now has the ability to play and fade out audio cues. However, it is currently limited to doing so at a fixed volume (and fixed fade-out times) until the audio pipeline gets redisigned (seriously, who thought it was a good idea to adjust the **SYSTEM** volume when changing the volume on a playbin??? I almost blew my speakers on that one...)

I have also started implementing context menues for cues depending on if they are stopped or playing/paused.

Up Next: Finalize the audio pipeline for this version and figure out how to get the tree view to live update with the playback progress.