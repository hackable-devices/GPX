
GPX
===
**Gcode to x3g conversion post processor.**


GPX is a post processing utility that converts GCode from 3D slicing software (like Slic3r and KISSlicer) into the x3g files used for standalone 3D printing on Makerbot Cupcake, ThingOMatic, and Replicator 1/2/2X printers. GPX output is compatible with both Makerbot and Sailfish firmware.

## Description


GPX is a fast and light weight program written in a structured programming style using ANSI C. GPX is precise and standards compliant in the x3g commands it outputs, and while it performs rigorous syntax and semantic error checking on the GCode input it interprets, GPX is very flexible and forgiving in the actual GCode it will accept.

GPX can be run from the command line, called by shell scripts or run as a post process. It has built-in support for 5D Cupcake, Thing-O-Matic and Replicator 1/2/2X printers. GPX can also load custom machine definitions if required. GPX configuration is very flexible, it can load a default configuration, be directed to load a custom configuration from the command line, or configured using a macro language embedded in the GCode header of the files it converts.


## History ##

### Version 1.3 (SEP 26, 2013)

Support for Cura was added. Reprap gcode flavor now interprets M106/7 as M126/7 (blower fan) to support Cura. There is also a new Cura python plugin script.

### Version 1.2 (AUG 24, 2013)

Added support for M133, M134, M135, M136 & M137 so gccode from Makerware converts without error. There is also a -g command line flag and gcode_flavor option to select Makerbot/ReplicatorG interpretation of M109.
GPX can be configured to perform convenient tasks like pause@zPos scripting, changing filament diameters without re-slicing, ditto printing with different filament diameters and varying the print temperature for wood filament.
