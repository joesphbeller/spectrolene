## Information about the data

The data cannot be shared because of copyright, but it is important to pay attention to the audio files you use to run your analyses.

This code is only compatible with **.wav mono** files.

You can follow this tutorial provided by [Apple][applemusic] to download your music as a .wav

In order to convert from **stereo** to **mono**, you can use *sox*

**Run the sox installation:**
Using Homebrew on Mac:
''' brew install sox  '''
or Linux
''' brew install sox  '''
or Python Package Index
''' pip install sox '''

**Average the channels in the stereo ([credit: linuxquestions.org])**
''' sox filename.wav -c 1 filename_mono.wav '''

Of course, this is not the only way. If you have a working way of converting stereo to mono, please share so we can help other users :)


[//] References

[applemusic]: <https://support.apple.com/en-us/HT204310>
[credit: linuxquestions.org]: <https://www.linuxquestions.org/questions/slackware-14/use-sox-to-make-a-file-mono-848072/>


