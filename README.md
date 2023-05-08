viless:  A tiny vi text editor clone with enough features to be truly useful


Adapted to run on bare metal: https://raymii.org/s/blog/Bare_Metal_Boot_to_Vi.html

~30 Kbyte executable size (32-bit ARM Linux gcc)

Copyright (C) 2000, 2001 Sterling Huxley <sterling@europa.com>

Revised:  5/18/20 by Brent Roman <brent@mbari.org>

Licensed under the GPL v2 or later

<pre>
Lifted from BusyBox 1.21
Modified to build stand-alone, fix bugs, improve status line display
30 Kb executable size on ARM with all features enabled
Lacks support for regular expressions
Implements only the most commonly used : commands

These features are available:
	Pattern searches with / and ?
	Last command repeat with '.'
	Line marking with 'x
	Named buffers with "x
	Readonly with -R command line arg
	Some colon mode commands with ':'
	Settable options with ":set"
	Signal catching- ^C
	Job suspend and resume with ^Z
	Adapt to window re-sizes

Things To Do:
	EXINIT
	$HOME/.exrc  and  ./.exrc
	add magic to search	/foo.*bar
	add :help command
	:map macros
	if mark[] values were line numbers rather than pointers
	   it would be easier to change the mark when add/delete lines
	More intelligence in refresh()
	":r !cmd"  and  "!cmd"  to filter text through an external command
	A true "undo" facility
	An "ex" line oriented mode- maybe using "cmdedit"
</pre>
