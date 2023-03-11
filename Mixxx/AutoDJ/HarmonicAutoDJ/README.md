# Updated Auto Harmonic DJ preset for Mixxx v2.3.0
This is an updated version of the Auto Harmonic DJ preset, which now works for Mixxx v2.3.0. It allows to beatmatch and also select musics based on their compatibility in line with harmonic mixing concepts.

I am not the original author, I just updated the preset to work with Mixxx v2.3.0 and fixed a few bugs (but not all! The preset is still very temperamental and then requires a full restart of the Mixxx app or at least disabling and reenabling the preset!).

More instructions are available at the top of the .js file.

Three configurations are provided:
* at root, the original updated by me, which was posted on the Mixxx forum at: https://mixxx.discourse.group/t/auto-dj-extension-for-beatmatching-and-harmonic-mixing/15962/35
* in MyConfig, a normal config I used at first, but which ended up having frequent playback issues, but is the most generalizable to any music style.
* in MyConfigRobust, a more robust config that reduces a lot the frequencies of playback issues, but sometimes they still happen, and then they require a restart of the Mixxx app. The trade-off for more robustness is that the preset is less adaptable to some music styles because it reduces the range of accepted bpm differences among other assumptions in parameters.
