## EASILY CREATE STUNNING ANIMATED CHARTS WITH CHART.JS

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with [Chart.js](https://www.chartjs.org/), a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

To see how to use chart.js we’re going to create a set of 3 graphs; one will show the number of buyers a fictional product has over the course of 6 months, this will be a line chart; the second will show which countries the customers come from, this will be the pie chart; finally we’ll use a bar chart to show profit over the period.

## Setting up

![chart](https://i.ibb.co/pPfd1jt/00.png)

## Drawing a line chart

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:
![canvas](https://i.ibb.co/4PS7s4T/01.png)
Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element:
![](https://i.ibb.co/qgvmppt/02.png)
