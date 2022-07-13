## Description 
A water Level senser that sense if the water level is below a preset setting. If the level dropes below the setting  
A light is turned on. When the water level rises back to its full state the bulb is turned off. 

## How it works
When the water dropes below a preset the upper level limit switch is opened and a lower level limit switch is actuated closed. A 5v DC signal 
is then sent to the set node of the SR NOR latch. The Q outut of the latch is then toggled high and latched on. This biases on an NPN transistor 
connecting one end of a relay to ground actuating the relays normally open switch thus tunring on a light bulb. 

When the water level rises back to the full state the lower level limit switch is opened and the upper level limit switch is closed.
A 5v signal is then sent to the SR NOR latch Reset node and the Q output is toggled low. This unbiases the NPN transisitor shutting off the relay  
and thus turning off the light bulb. 

## List of Components
