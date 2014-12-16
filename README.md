ViewshedMap
===========
A viewshed is the region visible to a point on a terrain. It is calculated by ray tracing to each point and checking for visibility, with some optimizations for speed.

A ViewshedMap generates a weighted map from a heights map (.dtm file format) where the values represent each points visibility (area of viewshed / maximum visibility).


## Usage

1. Import the ViewshedMap project into Eclipse.
2. Run KhTest as a Java Application

Options:
 *    single-click: clear all/reset display (also prints out data on point)
 * 	  double-click or 'v': toggle between source height map and viewshed heat map
 *    hold 'p' and single click: draw current perimeter (shows shape and size of last used setting)
 * 	  hold 'p' and drag mouse: set new perimeter size
 *    hold 'l' and drag line: draws rays, highlighting in light-blue the visible regions of the initial click
 *    hold 'm' and single click: highlights in blue the viewshed for that point
 *    hold 'm' and drag mouse: highlights viewshed of all points mouse touches

What you see is the viewshed weights map of test.dtm. By double clicking, or pressing `v` you can see the original heights map (green is lower altitude and red is higher altitude). Change the test.dtm file to a larger heights map file for more interesting results.
