---
title: ScatterSplineSeries
slug: chart-series-scatter-spline-series
---
# ScatterSplineSeries #

The **ScatterSplineSeries** are represented on the chart as data points connected with curved line segments. The **ScatterSplineSeries** inherit from the **[ScatterPointSeries]()** class and also require both axes of the chart to be of type **NumericalAxis**.

## Example ##
Here is an example of how to create a basic RadCartesianChart with ScatterSplineSeries in xaml:

	<telerikChart:RadCartesianChart>
	  <telerikChart:RadCartesianChart.BindingContext>
	    <viewMoedls:ScatterViewModel/>
	  </telerikChart:RadCartesianChart.BindingContext>
	  <telerikChart:RadCartesianChart.HorizontalAxis>
	    <telerikChart:NumericalAxis/>
	  </telerikChart:RadCartesianChart.HorizontalAxis>
	  <telerikChart:RadCartesianChart.VerticalAxis>
	    <telerikChart:NumericalAxis/>
	  </telerikChart:RadCartesianChart.VerticalAxis>
	  <telerikChart:RadCartesianChart.Series>
	    <telerikChart:ScatterSplineSeries ItemsSource="{Binding ScatterData}">
	      <telerikChart:ScatterSplineSeries.XValueBinding>
	        <telerikChart:PropertyNameDataPointBinding PropertyName="XValue"/>
	      </telerikChart:ScatterSplineSeries.XValueBinding>
	      <telerikChart:ScatterSplineSeries.YValueBinding>
	        <telerikChart:PropertyNameDataPointBinding PropertyName="YValue"/>
	      </telerikChart:ScatterSplineSeries.YValueBinding>
	    </telerikChart:ScatterSplineSeries>
	  </telerikChart:RadCartesianChart.Series>
	</telerikChart:RadCartesianChart>

Where:

	xmlns:telerikChart="clr-namespace:Telerik.XamarinForms.Chart;assembly=Telerik.XamarinForms.Chart"
Here is an example of how to create a RadCartesianChart with ScatterSplineSeries in code:

	var chart = new RadCartesianChart
	{
	    HorizontalAxis = new NumericalAxis(),
	    VerticalAxis = new NumericalAxis(),
	    BindingContext = new ScatterViewModel()
	};
	
	var series = new ScatterSplineSeries();
	series.SetBinding(ScatterSplineSeries.ItemsSourceProperty, new Binding("ScatterData"));   
	series.XValueBinding = new PropertyNameDataPointBinding("XValue");
	series.YValueBinding = new PropertyNameDataPointBinding("YValue");
	
	chart.Series.Add(series);


Here is the sample data:
	

![Basic ScatterSplineSeries]()
## Customization ##