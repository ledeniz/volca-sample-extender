#Volca Sample Extender  

This program extends the Korg Volca Sample MIDI functionality. There are already similar projects like this available but I wanted to make my own. Also I use a self written MIDI library, so be warned. 

## Features
* Play samples chromatically in a 4 octave range (MIDI channel 1-10)
* Play all the samples via notes on one channel from C-AS (MIDI channel 16)
* Pitch bend is translated to control the EG INT pitch parameter

## Usage
* Clone this repository
* Clone the BACH1 library in the lib/bach1
* Compile and upload to Arduino Uno (with the default IDE or PlatformIO)
* Hook up a MIDI I/O circuit

MIDI IN  -> RX (digital pin 0)
MIDI OUT -> TX (digital pin 1)

Make sure to use resistors and an optocoupler. A detailed circuit can be found here: http://www.instructables.com/id/Send-and-Receive-MIDI-with-Arduino/?ALLSTEPS

## Credits
Special thanks to Mauricio Maisterrena for the idea and his code. You can find his project here: https://github.com/mmaisterrena/Volca_Simple
