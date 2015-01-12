# Flite 2.0 for OS X
Basically a copy of the Flite 2.0 TTS engine, but with the Makefile fixed so it'll compile on OS X.

CMU made Flite, see more here:
http://www.festvox.org/flite/

## How to compile
First, you'll need the XCode Command Line Tools if you don't already have them installed.

Then:

1. Clone the repo to your own machine
2. Then do  `./configure`
3. Followed by `make`
4. And then finally `make install`

You should now be able to run flite from your command line. Try:

	flite -voice rms "Hello humans." -o test.wav && afplay test.wav

To generate a .wav file with the output, and then play it via afplay. For some reason directly routing the audio to the soundcard doesn't work for me.