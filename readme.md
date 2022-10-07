## disclaimer
This fork is intented to accumulate patches required to keep check_multi working in [https://github.com/ConSol/omd](OMD-Labs).
There is no support whatsoever.

## check_multi README

For the current documentation please see the [doc/readme.md](doc/readme.md)

## What is check_multi?

check_multi is kind of a wrapper plugin which takes benefit of the
Nagios 3.x capability to display multiple lines of plugin output.
It calls multiple child plugins and displays their output in the
long_plugin_output. A summary is given in the standard plugin output.

Normally the child return code with the highest severity becomes the
parent (check_multi) plugin return code. But you can influence this
by specifying flexible state evaluation rules.

The configuration is very simple: a NRPE-stylish config file contains
a tag for each child plugin and then the check command line.

## Author
Original author: Matthias.Flacke-at-gmx.de
