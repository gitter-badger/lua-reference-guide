<!-- This file was generated by the script. Do not edit it, any changes will be lost! -->

## playTone(frequency, duration, pause [, flags [, freqIncr]])



Plays a tone


#### Parameters

* `frequency` (number) tone frequency in Hz

* `duration` (number) length of the tone in (TODO units)

* `pause` (number) length of the pause in (TODO units)

* `flags` (number):
 * `0 or not present` play with normal priority.
 * `PLAY_BACKGROUND` play in background (built in vario function used this context)
 * `PLAY_NOW` play immediately

* `freqIncr` (number) positive number increases the tone pitch (frequency with time),
negative number decreases it. Bigger number has more effect



#### Return value

none

##### Notice
Minimum played frequency is 150Hz even if a lower value is specified.


