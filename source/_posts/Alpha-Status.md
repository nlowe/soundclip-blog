title: Alpha Status
date: 2015-03-01 21:28:32
tags: release
---

Well, here we are. It's been about two months since I've started on this project. Most of the functionality I wanted for the show that's coming up is there! I think it's at the point where I feel comfortable making the initial Alpha release!

### What does this mean?
I want to start using the [GitHub issue tracker](https://github.com/techwiz24/soundclip/issues) to start tracking problems that come up. After this post goes up, I'll start writing up some of the bugs that are present in this alpha.

Because it's an alpha, don't expect `master` to work 100% (or even 50%...) or be bug free. It definitely won't be. Once the software reaches the beta stage, master will be the `stable` or `release` branch, but until that point, it's the branch I'll actively develop on.

### So, is it ready for use in a production?
**NO!** Seriously, you probably want to stay away from using it in any semi-professional production at this point. It's not a [QLab](http://figure53.com/qlab) killer yet.

> Side rant: The QLab site doesn't support https. Seriously?

*Longer Answer*: Maybe. If you *really*, ***really*** want to use it. I intend on using it for an upcoming production in about four weeks time. I can't guarantee that it won't eat your project files, cues, or media. I can't guarantee it won't crash or start leaking memory mid-show. But I do know it works relatively well at this point in time. I plan on using these next four weeks to fix up bugs and improve stability. This means that I won't be adding **any new features** unless it's a feature I absolutely need for this upcoming production.

### Well then, how do I help?
You can help by completely disregarding what I just mentioned above! What I really need at this point are other eyes. What features do you need production to production? What currently implemented features don't function as expected or are straight up broken? I want this to be something that *every* Sound Designer can use in ***any*** production. I don't think you should have to have [expensive](http://store.apple.com/us/mac) hardware and software to professionally execute a production.

### Alright, alright, let me use it already!
Awesome! All you should need is `python3`, `python-gi`, `gtk3`, and `gstreamer`. Clone the project and execute the `soundclip` script in the root of the `src` folder and you'll be off to the races:

```bash
git clone https://github.com/techwiz24/soundclip.git
./soundclip/src/soundclip
```

You should also be able to download a tarball of the alpha [here](https://github.com/techwiz24/soundclip/releases/tag/v0.1.0-alpha1) if you don't want the git repository.

Make sure to save the project before trying to add audio cues! If I have any free time this week, I'll try to make a video to show people around.

### Next Steps
As mentioned above, I've got about three to three and a half weeks to stabilize and bugfix SoundClip. After the production is over (assuming the software survives the production), I want to make the interface nicer to use. Then, I want to try and bring it closer to feature parity with QLab (at least the audio portion). By next year, I want to have remote capibilities (D-Bus / OSC / MSC).

### Parting Notes
Currently I've got it configured to show all logging information by default. SoundClip will save the five most recent logs for any project with the project files. If your show runs for any decent length, this may end up taking up a lot of disk space. Because SoundClip will log to files and to `stdout` by default, you don't have to worry about saving console output if you encounter a problem. Just make sure to copy the log file from `.../.soundclip/logs/soundclip.log` somewhere safe to save it.

I hope others find this software useful. Break a leg!
