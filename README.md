# brightness

Shell script to adjust screen brightness from the command line, mainly intended for use with shortcut keys.

Designed for use on Pop!_OS (Ubuntu), but it should work in any environment that has `xrandr`. Automated default key binding setup requires Gnome. If you'd prefer different key bindings or are using a non-Gnome environment, you'll need to configure key bindings manually. Or you can just use the command line if you prefer.


## Installation

Open a terminal and paste the following command:

 	bash -c 'curl -o ~/.local/bin/brightness https://raw.githubusercontent.com/cfc23/brightness-cli/main/brightness && chmod +x ~/.local/bin/brightness'

This will download and install `brightness` in `~/.local/bin/` and mark it as executable. You can put it somewhere else if you want, but this location is a good default that should be in PATH on most systems, allowing `brightness` to work as a global command.

If you're using Gnome and you'd like the default key bindings (see below) to be automatically configured, type:

	brightness bindkeys


## Usage

	brightness [up|down|reset|bindkeys|<float>]
	   up       : Increase brightness by 0.1
	   down     : Decrease brightness by 0.1
	   reset    : Reset brightness to default
	   bindkeys : Set up default key bindings for Gnome (Alt+PageUp for up, Alt+PageDown for down, Alt+Home for reset)
	   <float>  : Set brightness to the specified value (e.g., 0.5)
