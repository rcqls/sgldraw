# sgldraw

`sgldraw` is a GPU accelerated, fairly performant, V module for
drawing vector shapes through `sokol.sgl`.

![screenshot](https://raw.githubusercontent.com/Larpon/sgldraw/master/img/screenshot.png)

The special thing about `sgldraw` is that it's real-time - meaning that it'll draw all
shapes from scratch 60 frames per second.

It also handles line widths > 1 - which makes the shapes look more like they'd do in
e.g. Inkscape. All shapes can also be animated with `sgl` transforms or by changing
each vertice coordinate the shapes is made up from.

## Dependencies
[earcut](https://github.com/Larpon/earcut)

## Why
It was an experiment on doing real-time vector graphics and also
to explore a way to package vector shape drawing into a self-contained
and standalone module.

For maintainance reasons `earcut` is an external dependency but it can
easily be distributed as a submodule to `sgldraw` if need be.

`sgldraw` has served as a personal playground but
I'm releasing it to the public in case some of the code might
be of interest to anyone.

## Notes
**The module not supported**
It's not completely abandoned but my focus is currently elsewhere
in V-land.

The example can be run with: `v run examples/app.v`
