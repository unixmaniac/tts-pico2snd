# tts-pico2snd
Modified TTS binary from SVOX

Original file was pico2wave which creates WAV files.
This is modified to output directly to the default audio device instead of a wav file.

# HOWTO build on Ubuntu
Make sure you have GCC installed.
You will need to install the following additional libraries

`sudo apt install libttspico-dev libpopt-dev libpulse-dev`

Compile with the following command

`gcc pico2snd.c -o pico2snd -lpopt -lpulse -lpulse-simple -lttspico`
