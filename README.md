![Project Cover](https://github.com/josephbeller/spectrolene/blob/master/img/spectrolene_cover.png)

# Spectrolene
**Spectrolene** is code originally intended for spectral analysis on a selection of Dolly Parton's music from her "Jolene" album. However, this code can be used on any music for audio analysis as long as the file type is a mono .wav. 

Check out my latest presentation on my analyis!
## Information about the data

The data cannot be shared because of copyright, but it is important to pay attention to the audio files you use to run your analyses.

This code is only compatible with **.wav mono** files.

You can follow this tutorial provided by [Apple][applemusic] to download your music as a .wav

In order to convert from **stereo** to **mono**, you can use *sox*
First, open a terminal [on Mac][l2] or [on Windows][l3]
**Run the sox installation:**
- Using Homebrew on Mac:
``` brew install sox  ```
- or Linux
``` brew install sox  ```
- or Python Package Index
``` pip install sox ```

**Average the channels in the stereo ([credit: linuxquestions.org])**\
``` sox filename.wav -c 1 filename_mono.wav ```

This can also be done in the **data** directory by running:
```./2mono.sh file_name```
Of course, this is not the only way. If you have a working way of converting stereo to mono, feel free to share, so we can help other users.

## Python installation
You can install the latest Python [here][l1]\
You can open a terminal [on Mac][l2] or [on Windows][l3]\
In terminal, install the following dependencies (or make sure they are installed):
```
pip install numpy
pip install matplotlib
pip install scipy
pip install librosa 
```
After downloading the files, you can run:
``` jupyter notebook ```
in terminal to open up a file navigation system with an integrated development environment (IDE) to handle the files.\
For the functions in the code to work without any modification to the code, add them to a folder named data that is located in the same directory as the .ipynb files. 

## Contact
For any troubleshooting, ideas, or suggestions:
**Joesph Beller**\
josdbell@vols.utk.edu\
josephbeller35@gmail.com

## Acknowledgements
A lot of help was provided by the Python, music, and audio communities:
 * [Top 3 Python packages to learn audio data science][l4]
 * [Learning from audio: the mel scale and mel spectrogram and mel frequency cepstral coefficients][l5]
 * Malawey, Victoria. A Blaze of Light in Every Word : Analyzing the Popular Singing Voice. New York, NY: Oxford University Press, 2020. Print.


[//]: #References

[applemusic]: <https://support.apple.com/en-us/HT204310>
[credit: linuxquestions.org]: <https://www.linuxquestions.org/questions/slackware-14/use-sox-to-make-a-file-mono-848072/>
[l1]: <https://www.python.org/downloads/>
[l2]: <https://www.youtube.com/watch?v=U8qQup7_nuo>
[l3]: <https://www.youtube.com/watch?v=8Iyldhkrh7E>
[l4]: <https://towardsdatascience.com/top-3-python-packages-to-learn-audio-data-science-project-cbd11c100fe7>
[l5]: <https://towardsdatascience.com/learning-from-audio-the-mel-scale-mel-spectrograms-and-mel-frequency-cepstral-coefficients-f5752b6324a8#:~:text=Leveraging%20Mel%20Spectrograms%20is%20a,learn%20from%20the%20recorded%20sounds.>

