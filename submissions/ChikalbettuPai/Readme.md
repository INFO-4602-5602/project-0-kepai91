# INFO 5602:  Project0


## Project Requirements:

The following parts and extra credits are completed :

Part 1: Interpreting Data

Part 2: Building Bars

Part 3: Building Scatterplots

Part 4: Interaction

Part 5: Building Multiple Charts


## Bells & Whistles:

Bell: Tooltips

The tooltip is displayed on mouse-hover over a data point.

Bell: Styling your Visualization (Done)

Used minimalistic black and white themed styling using [Bootstrap](http://getbootstrap.com/). Each question is represented in a panel-view.

Bell: Best Fit Lines

Tried to find the best fit line using least square coefficient. Reference to code snippets in [bl.ocks.org](http://bl.ocks.org/benvandyke/8459843) and  [stackoverflow](http://stackoverflow.com/questions/20507536/d3-js-linear-regression), but was unable to complete it. Therefore, have commented out the part.


## References:

1. [Simple Bar Chart Example](http://bl.ocks.org/d3noob/8952219)

2. [Scatter Plot example](http://bl.ocks.org/weiglemc/6185069)

3. [References to D3 Mouse Events](http://bl.ocks.org/WilliamQLiu/76ae20060e19bf42d774)

4. Reused some code snippets from the tutorial taught in class.

5. 





5.Selecting elements of multiple bar charts at the same time on Google groups

(https://groups.google.com/forum/#!topic/d3-js/cYnedmP54f0)

Used to highlight the related pair of bars at the same time which is task Whistle: Coordinated Views.

Pieces referred:

	var bar1 = svg.selectAll(".bar1")  //we select the related bar DOM based on the same class.
		.data(data).enter()
	 	.append("rect")
	 	.attr("class", function (d, i) { return 'bar' + i; })

	var bar2 = svg.selectAll(".bar2")
		.data(data).enter()
	 	.append("rect")
	 	.attr("class", function (d, i) { return 'bar' + i; })

	d3.selectAll('rect').on('mouseover', function() {
    	var rectClass = d3.select(this).attr('class');

    	d3.selectAll('.' + rectClass)    //controling the bars based on class will be effective
        	.attr('opacity', 0.2);

6.Part 2: Building Bars, Part 3: Building Scatterplots, part 4: interaction part and Bell:tooltips were implemented by using the code taught in class (tutorial code). To be more specific, we reused some of the code and made changes according to certain tasks.
