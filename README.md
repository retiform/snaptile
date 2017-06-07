# Snaptile

Versatile, mouse-free window tiling for X11.

![lol](https://user-images.githubusercontent.com/5866348/26905369-089db4d4-4bb5-11e7-90a8-96e39f278f1c.gif)

## Grid System

The grid system divides your screen into 12 sections

<kbd>ctl</kbd> + <kbd>alt</kbd> +


| <kbd>Q</kbd>| <kbd>W</kbd>| <kbd>E</kbd>| <kbd>R</kbd>|
|--|--|--|--|
| <kbd>A</kbd>| <kbd>S</kbd>| <kbd>D</kbd>| <kbd>F</kbd>|
| <kbd>Z</kbd>| <kbd>X</kbd>| <kbd>C</kbd>| <kbd>V</kbd>|

You can snap your window to any rectangle, of any arbitrary size, on this grid by specifying 2 corners. For example:

<kbd>ctl</kbd> + <kbd>alt</kbd> + <kbd>E</kbd> + <kbd>D</kbd>

| x | x | <kbd>E</kbd>| x |
|--|--|--|--|
| x | x | <kbd>D</kbd>| x |
| x | x |      x      | x |


Which looks like

![screenshot from 2017-06-07 18-50-28](https://user-images.githubusercontent.com/5866348/26905371-0b657a26-4bb5-11e7-9e0f-b3a56f5802a5.png)


## Requirements
* Python3
* X11-based desktop
* python3-gi
* python3-xlib

## Installation on Ubuntu
```bash
$ sudo apt-get install git python3-gi python3-xlib
$ cd <place-you-want-to-store-pygrid>
$ git clone https://github.com/mjs7231/pygrid.git
$ cd pygrid && ./pygrid.py
```

To start at boot, just add a script to *Startup Applications* invoking the python script
```bash
/usr/bin/python3 <full-path>/snaptile/snaptile.py
```

## Credits
Snaptile is a rewrite of [PyGrid](https://github.com/pkkid/pygrid), supporting the more powerful shortcuts system.