# 3DSurfaceThing

**Disclaimer**

This repository is provided "AS-IS" with **no warranty or support** given. This is not an official or supported product/use case. 



**Description**

This repo contains instructions on how to plot a 3D surface and display it in a mashup. It contains:

* an example dataset (plotly3Datatable) and a sample mashup (plotlyTest).
* the build artifacts for [ThingworxPlotlyChartingSDK](https://github.com/jmccuen/ThingworxPlotlyChartingSDK)  and  [ThingworxPlotlyExamplePlots](https://github.com/jmccuen/ThingworxPlotlyExamplePlots) 

This guide leverages the work of [jmccuen](https://github.com/jmccuen) who implemented the [plotly](https://plot.ly/javascript/) javascript library using the [Thingworx Java SDK](https://marketplace.ptc.com/apps/193544/extension-sdk-v83#!overview). The PlotlyExamplePlots extension also contains implementations for other graphs:

* Timeseries Plot
* Label Plot
* Pie Plot
* and Surface Plot which we are demonstrating here. 



### Configuration

* Import the [PlotlyChartLibrary-dev-1.0.192.zip](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/PlotlyChartLibrary-dev-1.0.192.zip) first, into Thingworx, then import [PlotlyPlots.zip](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/PlotlyPlots.zip). 
* Import the example [datashape](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/DataShapes_plotly3Datashape.xml), [datatable entity](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/Things_plotly3Datatable.xml), [datatable data](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/plotly3Datatable-Data.zip), and then the mashup [plotlyTest](https://github.com/ptc-iot-sharing/3DSurfaceThing/blob/master/Mashups_plotlyTest.xml).

You can now view the 3D surface plot inside the example mashup or create your own plot, using the Surface Plot widget, that should now appear in the widget picker.



### Data

As you will see from the sample data table included, or the sample data from [Plotly](https://raw.githubusercontent.com/plotly/datasets/master/api_docs/mt_bruno_elevation.csv), the format required for this type of plot to work is a grid pattern (x,y) and the elevation (z). 

The first column will be y, from 0 to 24 for example. The first row will be x, starting with 0 in column 2, i.e. for each intersection of [x,y] you will have height z. 

You can also check out the [sample Js](https://plot.ly/javascript/3d-surface-plots/) available from Plotly.



### Functionality

The [Topographical 3D Surface Plot](https://plot.ly/javascript/3d-surface-plots/#topographical-3d-surface-plot) is the type implemented in this version. More [3D charts](https://plot.ly/javascript/#3d-charts) can be implemented by modifying the Surface Plot code  [ThingworxPlotlyExamplePlots](https://github.com/jmccuen/ThingworxPlotlyExamplePlots)/[ui](https://github.com/jmccuen/ThingworxPlotlyExamplePlots/tree/master/ui)/**surfaceplot**/ . 
