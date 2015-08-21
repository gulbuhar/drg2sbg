This program converts the .drg propiatary file format into the open source SBaGen format.

I-Doser is a company that produces Binaural brainwaves to simulate different states.

The problem is that they don't provide a doser application for Linux, and their mp3 collection is limited, with this program you can convert the .drg file to an .sbg and then using [SBaGen](http://uazu.net/sbagen/) (an open source application that they use as main engine to generate the tones) you can convert it to wav and (if desired) to mp3 or similar.

This project will never be possible without the help of ["The Unofficial I-Doser Blog"](http://theidoserblog.blogspot.com/) and their steAlth's DRG Author by konstAnt and khAttAm to tell the truth this is a rip off stripped version of konstAnt and KhAttAm steAlth's DRG Author. They did all the work with the .drg files, I just port some parts of it to C.

Features:
  * Convert drg file into sbagen format
  * Extract every part of the drg file (description, title, image, sbagen code)
  * Create drg files

Documentation:
  * [Compilation and installation notes](CompilationInstallation.md)
  * [Usage notes](Usage.md)
  * [Instructions to make mp3 files](ToMP3.md)