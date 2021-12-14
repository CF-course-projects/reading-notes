<p></p>
<ul>
<li></li>
<li></li>
<li></li>
</ul>
<p>Charts with chart.js</p>
<ul>
<li>after downloading and importing in Charts.js, create a script tag  with a source attribute with Chart.min.js</li>
<li>To draw a line chart: make a canvas tag, with id, width and height attributes</li>
<li>make a js var to save the reference to the canvas element: var buyers = document.getElementById('buyers').getContext('2d');</li>
<li>make a new chart using the new keyword: new Chart(canvas var).Line(object with data)</li>
<li>Making a pie chart:<ul>
<li>create canvas tag in html</li>
<li>make a js var to save the reference to the canvas element</li>
<li>call the chart function: new Chart(countries).Pie(pieData, pieOptions);</li>
<li>pass in an object(pieData) holding data and another(pieOptions) </li>
<li>var pieOptions = {
	segmentShowStroke : false,
	animateScale : true
}</li>
</ul>
</li>
<li>Making Bar Charts:<ul>
<li>create canvas tag in html</li>
<li>make a js var to save the reference to the canvas element</li>
<li>call the chart function: new Chart(income).Bar(barData);</li>
<li>pass in both the window into the DOM and the object holding the data</li>
</ul></li>
</ul>
