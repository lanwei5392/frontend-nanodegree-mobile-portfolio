---------------------------
Running this Application
---------------------------

Open the url link for the gh-pages from the repository in github. https://lanwei5392.github.io/frontend-nanodegree-mobile-portfolio/

----------------------------------------------------------------
Optimizations made to index.html to achieve PageSpeed score > 90
---------------------------------------------------------------

The pageSpeed for pizza landing page(index.html) has reached 96 for mobile and 97 for desktop. 

The following optimizations are used to improve the pageSpeed.
-Used inline CSS, which is to use the codes defiend in style.css to repplace the related style lines in index.html
-Used inline JS, which is to use the codes defined in perfmatters.js to replace the related codes in index.html
-Replaced Cam's pizzeria image by a compressed image which is newly loaded views/images/pizza.jpeg. 

 --------------------------------------------------------
 Optimizations made to views/js/main.js to achieve 60 FPS
 --------------------------------------------------------

 +In the updatePositions() function on line 519, the phase calculation 
 +results were placed into an array, which is then called by a for loop, 
 +so the calculation will not be performed each iteration.
 +
 +In the for loop on line 568, the max value of i was converted to the
 +value of the screen height multiplied by var row times var cols.
 +
 +All querySelector tags were converted to getElementById or 
 +getElementsByClassName.
 +
 +Calculations and variable declarations nested inside for loops were 
 +moved into local variables that are then called inside the for loop.
