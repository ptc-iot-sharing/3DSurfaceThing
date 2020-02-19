# 3DSurfaceThing

This repo contains instructions on how to plot a 3D surface and display it in a mashup. It contains:

* an example dataset (plotly3Datatable) and a sample mashup (plotlyTest).
* the build artifacts for [ThingworxPlotlyChartingSDK](https://github.com/jmccuen/ThingworxPlotlyChartingSDK)  and  [ThingworxPlotlyExamplePlots](https://github.com/jmccuen/ThingworxPlotlyExamplePlots) 

This guide leverages the work of [jmccuen](https://github.com/jmccuen) who implemented the [plotly](https://plot.ly/javascript/) javascript library using the [Thingworx Java SDK](https://marketplace.ptc.com/apps/193544/extension-sdk-v83#!overview). In the PlotlyExamplePlots there are implementations additional graphs:

* Timeseries Plot
* Label Plot
* Pie Plot
* and Surface Plot which we are demonstrating here. 



### Configuration

* Import the ThingworxPlotlyChartingSDK first, into Thingworx, then import ThingworxPlotlyExamplePlots. 
* Import the example datatable entity, plotly3Datatable, and then the mashup plotlyTest.

You can now view the 3D surface plot inside the example mashup or create your own plot, using the Surface Plot widget, that should now appear in the widget picker.



### Data

As you will see from the sample data table included, or the sample data from [Plotly](https://raw.githubusercontent.com/plotly/datasets/master/api_docs/mt_bruno_elevation.csv), the format required for this type of plot to work is a grid pattern (x,y) and the elevation (z). 

The first column will be y, from 0 to 24 for example. The first row will be x, starting with 0 in column 2, i.e. for each intersection of [x,y] you will have height z. 

You can also check out the [sample Js](https://plot.ly/javascript/3d-surface-plots/) available from Plotly.



### Functionality

The [Topographical 3D Surface Plot](https://plot.ly/javascript/3d-surface-plots/#topographical-3d-surface-plot) is the type implemented in this version. More [3D charts](https://plot.ly/javascript/#3d-charts) can be implemented by modifying the Surface Plot code  [ThingworxPlotlyExamplePlots](https://github.com/jmccuen/ThingworxPlotlyExamplePlots)/[ui](https://github.com/jmccuen/ThingworxPlotlyExamplePlots/tree/master/ui)/**surfaceplot**/ . 