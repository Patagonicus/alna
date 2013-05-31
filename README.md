Alna
====

Alna is a small script that generates a large image of nyan cat and splits it into smaller images that can each be displayed on one screen. It's still work in progress, lacks some features and has little to no error checking, but it should be useable.

Dependencies
------------
Alna extensively uses ImageMagick. If (GNU) parallel is found it is used to speed up the stitching progress for the backrgound on multicore systems, but it also works without parallel.

Usage
-----

    alna screen1 [screen2 […]]

Just pass alna the sizes of the displays in pixels from left to right. Use "x" as a delimiter between the width and height, e.g. 1920x1080 for Full HD. The resulting images will be named nyan0.png, nyan1.png, … in the current working directory.
