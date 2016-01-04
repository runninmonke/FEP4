## Website Performance Optimization portfolio project

This is a portfolio website that had a number of performance issues. They were primarily found on index.html and views/pizza.html.

I improved the PageSpeed score of index.html by doing the following:
* Moved some CSS into non-render blocking style sheets
* Inlined the remaining CSS
* Removed Google Fonts link
* Made Google analytics javascript load asyncronously
* Optimized image files

I improved the rendering of views/pizza.html by removing "jank" in the following ways:
* Limited the number of background pizzas created to only those that will fit within the screen height
* Changed CSS effect used to implement pizza animation to 'transform: translateX' to avoid Layout recalculations
* Moved computational work that remains unchanged each iteration to the outside of the 'for' loops in 'changePizzaSizes' and 'updatePositions'

#### Getting Started
Simply navigate to http://runninmonke.github.io/FEP4/ or launch index.html.
