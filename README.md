# sxmo-alarm
Script to install [sxmo](https://sr.ht/~mil/Sxmo/) onto an [Arch Arm barebones image](https://github.com/dreemurrs-embedded/Pine64-Arch/releases). 
If this script helps you then please consider buying me a coffee or two ;)

<a href="https://www.buymeacoffee.com/JustineSmithies">Buy me a coffee</a>

![ScreenShot](screenshot.jpg)

The wallpaper is available [here](https://www.artstation.com/artwork/gJPLLx)

## To install and run:

Copy sxmo-alarm somewhere in either the root of your home directory 
or some other directory under your home on your Pinephone and

chmod +x sxmo-alarm

sudo ./sxmo-alarm from the directory that you installed it.

## Notes: 

Running this script periodically will update sxmo from git.

I've also supplied my .Xresources ( Gives the yellow / black theme ), picom.conf and modified conky.conf .

Also if you do use picom for transparency then it will severely impact the performance of the Megapixels camera to the point of unuseability. Not sure of a workaround as yet ?

If you'd like feedback on keypresses then put this line in your ~/.profile

export KEYBOARD_ARGS="-o | clickclack -V -f wavfile.wav"

Remove the -f and filename if you just want vibration. More details on clickclack are [here](https://git.sr.ht/~proycon/clickclack)

## Issues

Firefox sets layout.css.devPixelsPerPx set to -1.0 on Arch for some reason which cause it to display too big.
To resolve this type about:config in the url bar and search for layout.css.devPixelsPerPx then change it to 1.0


## User Manual:

The user manual is located [here](https://git.sr.ht/~mil/sxmo-docs/tree/master/USERGUIDE.md)
