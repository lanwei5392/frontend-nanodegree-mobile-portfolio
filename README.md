------------------------
Running this Application
------------------------

Open the url link for the gh-pages from the repository in github. https://lanwei5392.github.io/frontend-nanodegree-mobile-portfolio/

-----------------------------------------------------------------
Optimizations made to index.html to achieve PageSpeed score > 90
-----------------------------------------------------------------

The pageSpeed for pizza landing page(index.html) has reached 96 for mobile and 97 for desktop. 

The following optimizations are used to improve the pageSpeed.
-Used inline CSS, which is to use the codes defiend in style.css to repplace the related style lines in index.html
-Used inline JS, which is to use the codes defined in perfmatters.js to replace the related codes in index.html
-Replaced Cam's pizzeria image by a compressed image which is newly loaded views/images/pizza.jpeg. 

 --------------------------------------------------------
 Optimizations made to views/js/main.js to achieve 60 FPS
 --------------------------------------------------------

1. To achieve 60 FPS for scroll pizza page - 

Line-527, reduced the total of background pizzas by changing i from 200 to 24. 
Line-507 to Line-520, resolved forced reflow by setting up a phase array out of the style loop to avoide calculating layout at each step in the loop. 
Line-473, declared PizzaDiv out of the loop.
In multiple areas, replaced querySelector tags by getElementById or getElementsByClassName.

2. To achieve 60 FPS for sliding pizza size

Line 452-462, resolved forced reflow by setting up allRandomPizzaContainers, dx and newwidth out of the loop to avoid recalculating layout at every step.
Line-433 to Line-466, in the middle of changing pizza size and define all pizza size array.
