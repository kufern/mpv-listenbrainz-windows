# mpv-listenbrainz-windows
A Windows script to submit mpv listens to ListenBrainz

**FULL DISCLOSURE:** I used ChatGPT to help make this script. If you are not okay with using clanker-written code, feel free to ignore this and carry on. I will probably go back and fix this up when I get better at this.

This script was originally made by Alexandre Rousseau (madeindjs) [[link](https://gist.github.com/madeindjs/f33225cf4d8fdc9f61e0fe3ebe2dcce7)]. I have retooled it in order to make it work on Windows

----
# Installation
To download the file, go to [the file](/blob/main/mpv-listenbrainz.js) and click on the download button.

Then, put it in the mpv \scripts folder. This will either be at "%APPDATA%\mpv\scripts\" or "\apps\mpv\current\portable_config\scripts" if you are using [scoop](https://scoop.sh) (**NOTE:** You will have to make the folder if it's not there)

Finally, open Powershell and run this:
```
setx LISTENBRAINZ_USER_TOKEN "<token>"
```
To get your token, go to https://listenbrainz.org/settings/

**Close that Powershell windows and mpv**, then open it back up. Run `$env:LISTENBRAINZ_USER_TOKEN` to check if your token has been set.

Run `mpv <insert song location>` to see if its working. After this, you can use the GUI like normal.
