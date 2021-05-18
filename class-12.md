# Lecture Notes 12

## Topics on Canvas API
- Basic Usage
- Drawing shapes with canvas
- Applying styles and colors
- Drawing text

### Charts
- Charts are better for displaying data visually than tables at times.
- Easier to look at and convery data quickly, but not always easy to create.
- Using Chart.js is easiest. A javascript plugin that uses cavas elements

## Chart JS

### Setting up
- Download Chart.js. Copy chart.min.js out of folder.
- create new HTML and import:

``` js
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>
```

### Drawing line chart
``` js
<canvas id="buyers" width="600" height="400"></canvas>
// next, write a script that will retrive the context of the canvas, add this to the foot of body element.
<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>
```
- Create the data inside the script tags.
``` js
var buyerData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "rgba(172,194,132,0.4)",
			strokeColor : "#ACC26D",
			pointColor : "#fff",
			pointStrokeColor : "#9DB86D",
			data : [203,156,99,251,305,247]
		}
	]
}
```

### Pie Chart
``` js
//canvas
<canvas id="countries" width="600" height="400"></canvas>

// context and instatiating the chart
var countries = document.getElementById("countries").getContext("2 new Chart(countries).Pie(pieData, pieOptions)")

// supply value data for the pieData
var pieData = [
	{
		value: 20,
		color:"#878BB6"
	},
	{
		value : 40,
		color : "#4ACAB4"
	},
	{
		value : 10,
		color : "#FF8153"
	},
	{
		value : 30,
		color : "#FFEA88"
	}
];
// and then options
var pieOptions = {
	segmentShowStroke : false,
	animateScale : true
// The options above remove the stroke from the segments, and animate the sclae of the pie so that it zooms out from nothing.
}
```

### Bar Chart
``` js 
<canvas id="income" width="600" height="400"></canvas>

var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);

var barData = {
	labels : ["January","February","March","April","May","June"],
	datasets : [
		{
			fillColor : "#48A497",
			strokeColor : "#48A4D1",
			data : [456,479,324,569,702,600]
		},
		{
			fillColor : "rgba(73,188,170,0.4)",
			strokeColor : "rgba(72,174,209,0.4)",
			data : [364,504,605,400,345,320]
		}
	]
}

//supplying the data for the bar chart.
```
