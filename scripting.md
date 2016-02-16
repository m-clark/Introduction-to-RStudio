Scripting
========================================================
author:
date: 2016-02-14
autosize: true
transition: concave
css: csstestCSStherealCSSSERIOUSLY.css
font-family: 'Helvetica'



Scripting
========================================================

Everyone that uses Rstudio does so for easier scripting, including:

- Syntax highlighting
- Autocomplete of object/function names, etc.
- Autopairing of parenthesis, quotes etc.
- Auto indent

It even makes working at the console viable

- Still not advised



Keyboard shortcuts: standard scripts
========================================================
left: 60%
Knowing a few <span class="emph">shortcuts</span> can save *a lot* of time in the long run.

Examples (Windows and Linux):
Run current line: Ctrl+Entr

Run up to/from current line: Ctrl+Alt+B/Ctrl+Alt+E

Run everything: Ctrl+Shft+Entr

Insert section: Ctrl+Shft+R
***
<img src="img/keyboardsc.png" style="display:block; margin: 0 auto;">
<div style="text-align:center">Alt+Shft+K</div>

Keyboard shortcuts: standard scripts
========================================================
Copy up/down: Ctrl+Shft+up/down

Move up/down: Shft+up/down

Yank up to cursor: Ctrl+u

Yank after cursor: Ctrl+k

Select multiple lines: Ctrl+Alt+Click

Select Window: Ctrl+1:9

Expand Window: Ctrl+Shft+1:9



Keyboard shortcuts: tabs
========================================================
Previous tab: Ctrl+F11

First tab: Ctrl+Shft+F11

Next tab: Ctrl+F12

Last tab: Ctrl+Shft+F12



Keyboard shortcuts: documents
========================================================
Insert Chunk: Ctrl+Alt+i

Run Chunk: Ctrl+Alt+c

Run previous chunks: Ctrl+Alt+p

Knit document: Ctrl+shft+k



Keyboard shortcuts
========================================================

The point is, knowing just a dozen shortcuts could save a lot of time.

Bonus: Ctrl+Shft+a (tidy up your code)

Mac users: most of these would use Cmd rather than Ctrl (but not always)



Snippets
========================================================
left: 60%

Snippets allow one to insert code of a certain form for certain commonly used functions.

- For loops, apply family, etc.

You only have to type the first couple letters, the form of the rest of the code will fill out, then you can tab your way through the rest of it.



```r
name <- function(variables) {

}

for (variable in vector) {

}

apply(array, margin, ...)
```

***
<img src='img/snippet1.png' style='width:150%; height:200%'>
<img src='img/snippet2.png'>


Code Diagnostics
========================================================
left:50%
Rstudio will note problems in your code in the margin

- Examples: hanging brackets, too many commas etc.

This works beyond just R scripts too
***
<img src="img/codediagnosticcss.png" style="display:block; margin: 0 auto;">



