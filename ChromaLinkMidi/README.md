# Python script for automatic beatmatched light show with RazerChroma/ChromaLink compatible light devices

I’ve made two years ago an automatic music and lights show for a party. For the music part, i have updated the Auto Harmonic DJ plugin (see my other posts - but compatibility may be broken nowadays). For the light show part, I used a Yeelight 1S which offers compatibility with Razer Chroma Connect and ChromaLink (another tool that Yeelight provides to connect to Razer Chroma Connect).

Then, in Mixxx, in Controllers > (name of midi loopback device), set Load Mapping to “MIDI for light” to send midi events in rhythm to a midi loopback device (such as LoopBe1 on Windows).

Finally, this loopback device can be used by your own script to send light commands to ChromaLink and Razer Chroma Connect. This is the purpose of my Python script, that I share with you today.

Note that it was made and tested on Mixxx v2.3.0, although it should work with newer releases since it does not interact directly with Mixxx but with the mitdi events.

The script is a Jupyter notebook and it requires a few modules to be able to receive midi events. Its functeons are relatively basic, as it switches color in rhythm with the music, according to a predefined pattern. This can easily be extended to more dynamical or complex patterns, ant multiple lights can be controlled simultaneously.

Overall, it’s a great way to get into light shows for a cheap price, as a Yeelight 1S only costs 20-30 bucks and it can be controlled via wifi, no need for complex setups and there is no hub.

Note that an alternative is to use Razer Chroma Connect integrated music visualization feature, but it is very imperfect since it uses frequency analysis to try to find the music’s rhythm, whereas here we directly get the beat from midi events so the accuracy is unbeatable, and also we get a lot finer control over the light color and intensity.

Tl;dr, this is a very simple script not meant to do anything fancy but it may help others get started with cheap light shows system using razer chroma systems and Mixxx. Have fun!

Forum announcement and comments: https://mixxx.discourse.group/t/automatic-beatmatched-light-show-with-razerchroma-compatible-chromalink-python-script/26854/1
