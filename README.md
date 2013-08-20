brawl4d
=======

Interactive four-dimensional (space and time) data browsing using the stormdrain data processing pipeline. When data are loaded, they are pushed downstream to plot outlets, stdout, etc. Along the way, data may be transformed, filtered, cached, and branched off to other analysis tasks, including other plots beside the main viewer. There is also animation support.

The interactivity is provided graphically by interaction with plots in matplotlib, and via the command line using the IPython notebook, of which there are several examples in brawl4d/notebooks. As the IPython notebook gains browser-based GUI capabilities, it should be possible to replace code cells that trigger, for instance, animation, with buttons and other standard UI conventions.

It should be trivially easy to add any dataset that is represented as a numpy structured/named array (see the demo dataset in brawl4d.py). Times are treated as seconds since a reference date, which is stored as the basedate attribute of the Panels4D object. Adding radar data viewing capability, probably through pyart, is a high priority.


Requirements
------------

- Python
- IPython
- numpy and matplotlib
- stormdrain (github.com/deeplycloudy/stormdrain)
- For LMA support
    - lmatools (bitbucket.org/deeplycloudy/lmatools)
    - pytables (for HDF5 LMA data files)

Install
-------
Clone and add to your path. Adding a proper setup.py is a TODO.


What's with the name?
---------------------
Balloon, Radar, and Aircraft, With Lightning in Four Dimensions.