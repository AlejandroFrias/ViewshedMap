ViewshedMap
===========
A viewshed is the region visable to a point on a terrain. It is calculated by ray tracing to each point and checking for visability, with some optimizations ofr speed.

A ViewshedMap generates a weighted map from a hights map (.dtm file format) where the values represent each points visability (area of viewshed / maximum visibility).
