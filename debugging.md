Debugging
========================================================
author:
date: 2016-02-18
autosize: true
transition: linear
transition-speed: fast
css: workshop.css
font-family: 'Helvetica'

What is Debugging?
========================================================

Debugging is merely finding and fixing problematic code.

  - Code will always have bugs

Debugging is an absolutely essential part of creating functions.

Debugging in RStudio
========================================================

There are numerous facilities within R to help you debug your code.

As with everything, RStudio makes the whole process easier.

 - RStudio also has numerous facilities for debugging.


Overview
========================================================
incremental: true

Break Points

<span class="func">browser()</span>

<span class="func">debugonce()</span>



Breakpoints
========================================================

Editor breakpoints are used to enter into debugging at a certain line.

Breakpoints are created by clicking next to a line number in a function.

You must <span class="func">source()</span> the function before the breakpoints will be implemented

browser()
========================================================

Used to stop a function at a certain point and enter into debugging.

  - Essentially a hard-coded editor breakpoint


```r
wackyAvg = function(a, b, c, d, e, f) {
  resSum = (a * .5) + (b * 2.5) + (c * 4.5) + (d * 6.5) + (e * 8.5) + (f * 10.5)
  browser()
  wackAvg = resSum / 6
  print(wackAvg)
}
```

debug() and debugonce()
========================================================

As opposed to specifying breakpoints or including a <span class="func">browser()</span> line, <span class="func">debug()</span> will start from the top and work through each line.

The <span class="func">debug()</span> function will run everytime you run the function.

  - You will have to <span class="func">undebug()</span> to break this behavior

Using <span class="func">debugonce()</span> will keep that loop from starting.


debug()
========================================================


```r
wackyAvg = function(a, b, c, d, e, f) {
  resSum = (a * .5) + (b * 2.5) + (c * 4.5) + (d * 6.5) + (e * 8.5) + (f * 10.5)
  wackAvg = resSum / 6
  print(wackAvg)
}

debug(wackyAvg)

wackyAvg(1, 2, 3, 4, 5, 6)

undebug(wackyAvg)
```


debugonce()
========================================================


```r
wackyAvg = function(a, b, c, d, e, f) {
  resSum = (a * .5) + (b * 2.5) + (c * 4.5) + (d * 6.5) + (e * 8.5) + (f * 10.5)
  wackAvg = resSum / 6
  print(wackAvg)
}

debugonce(wackyAvg)

wackyAvg(1, 2, 3, 4, 5, 6)
```


Debug Mode Commands
========================================================
incremental: true
left: 50%

There are commands that allow you to work through debugging:

Next (n): runs the next line

Step into (s): if the next line is a new function, it enters into the function

Finish (f): finishes the function

Continue `(c)`: stops debugging and runs the function

Stop (Q): stops debugging and does not run the function

***

Each of these also has a button in the debugging menu

<img src="img/debugToolbar.png" style="display:block; margin: 0 auto;">

Quick Wrap
========================================================
incremental: true

Debugging is an important part of programming.

RStudio makes the debugging more interactive and flexible than R alone.
