# ExyGraph
A lightweight graphing library written in Swift

## Installation ##
To use ExyGraph, just drop `ExyGraph.swift` anywhere in your project.

## Using ExyGraph ##
1. In your storyboard, drag a plain view on to you view controller.
2. Rename its class to `Graph` in the IB sidebar. When the file builds again, you'll see a default blue graph in the view.
3. ExyGraph makes use of the new `@IBDesignable` functionality. Many attributes of your graph can be customized directly from the IB sidebar.

## Adding Data ##
ExyGraph currently only draws XY line graphs in a similar style to the iOS Health app. Each `Graph` contains an array of `Plot` objects, which define the characteristics of the plot. Each `Plot` contains an array of `Point` objects, where the actual data is stored. The X-Coordinate data in a `Point` can be any object of your choosing. ExyGraph does not sort any of the data. It will present in exactly the order the data is placed. 

## Future Updates ##
The X-Coordinate data currently converts integers in the range 0-11 to their corresponding month for labelling on the X-axis. This specific implementation will be the first thing to be abstracted away.
