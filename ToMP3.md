# Convert to mp3 #

It is possible to convert the output of SBaGen to an mp3 file, however you need to be sure to preserve the stereo separation.

Options like mono and joint stereo will not work.

I recommend to read the documentation of your encoding application.

This is how i do it (using lame)

```
drg2sbg -o file.sbg file.drg
sbagen -o file.wav -W file.sbg
lame -m s -V 0 file.wav file.mp3
```