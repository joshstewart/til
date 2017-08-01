### When audio isn't working, e.g., volume controls don't do anything or there is no audio

In a Terminal window and run:

`sudo killall coreaudiod`

You may also need to run the following two commands right after:

`sudo kextunload /System/Library/Extensions/AppleHDA.kext`

`sudo kextload /System/Library/Extensions/AppleHDA.kext`

[Source](https://apple.stackexchange.com/questions/124476/unable-to-modify-the-volume-with-the-keyboard)
