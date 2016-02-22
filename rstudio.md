Doing More with Rstudio
========================================================
author:
date: 2016-02-22
autosize: true
transition: concave
css: workshop.css
font-family: 'Helvetica'

Outline
========================================================
## Overview
## Scripting
- Common Shortcuts
  - Cleaner code
  - Moving around
- Customization

## Project Management
## Documents
-  Templates

Outline
========================================================

## Presentations (like this!)
## Version control
## Addins
## Cheatsheets

Outline
========================================================

## Advanced
- Other programming languages
- Deubgging
- Package development

Who this is for
========================================================
People who currently use Base R's text editor

People who use Rstudio only for scripting purposes

Possibly those who use the more powerful text editors and wonder what the fuss is about


Overview
========================================================
author:
date: 2016-02-22
autosize: true
transition: concave
css: workshop.css
font-family: 'Helvetica'



Overview
========================================================

Base R is an extremely powerful tool

The syntax editor in Base R is awful

You should use something more efficient and easy to use

Options:

- Rstudio
- Emacs
- Vim
- Various others



Overview
========================================================
Rstudio's strength is in assuming an interactive session from the outset

Emacs is especially powerful and useful (though at its core, a text editor rather than IDE)

- Some of the R-core maintain Emacs Speaks Statistics

However, there is an Emacs (and Vim) mode within Rstudio

- Bring that editing approach to Rstudio with you

You still might want RStudio for documents/presentation

- $\LaTeX$ isn't everything



Overview
========================================================
transition: fade
Rstudio offers:

- Code completion and snippets
- Code diagnostics
- Customizable shortcuts
- Document generation (web, pdf, presentation, .doc)

    -Spell check

- Web publishing

Overview
========================================================
transition: fade
Rstudio offers:

- Enhanced debugging
- Navigable data frames
- Version control
- Interactive visualization
- Addins


Overview
========================================================
Rstudio is an excellent tool for reproducible research

- Project management
- Package building and freezing
- Document generation

In short, you can go from data import to (modern, web-based) publication and replication


Scripting
========================================================
type:prompt

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




