<style>
.footer {
    color: black;
    background: #E8E8E8;
    position: fixed;
    top: 90%;
    text-align:center;
    width:100%;
}

.reveal h1, .reveal h2, .reveal h3 {
  word-wrap: normal;
  -moz-hyphens: none;
}
</style>

From experimental data to plots
========================================================
author: Maciej Dobrzynski
date: August 21, 2019
autosize: true

RStudio Projects
========================================================
Divide your work into multiple contexts with RStudio projects.

Each project has its own working directory, workspace, history, and source documents.

You can create an RStudio project:

   - In a brand new directory
   - In an existing directory where you already have R code and data
   - By cloning a version control (Git or Subversion) repository
   
File > New Project... to create a new R project


Code formatting
===============
When working in RStudio with regular R scripts, use # to add comments to your code. Additionally, any comment line which includes at least four trailing dashes (-), equal signs (=), or pound signs (#) automatically creates a code section. For example, all of the following lines create code sections.

Note that the line can start with any number of pound signs (#) so long as it ends with four or more -, =, or # characters.

To navigate between code sections you can use the Jump To menu available at the bottom of the editor. You can expand the folded region by either clicking on the arrow in the gutter or on the icon that overlays the folded code.

RStudio supports both automatic and user-defined **folding** for regions of code. Code folding allows you to easily show and hide blocks of code to make it easier to navigate your source file and focus on the coding task at hand.

To indent or reformat the code use:

   - Menu > Code > Reindent Lines (⌘I)
   - Menu > Code > Reformat Code (⇧⌘A)

Syntax convention
=================
It is a good practice to stick to a single naming convention throughout the code. A convenient convention is a so-called [camel notation](https://en.wikipedia.org/wiki/Camel_case#Programming_and_coding), where names of variables, constants, functions are constructed by capitalizing each comound of the name, e.g.:

   - `calcStatsOfDF` - function to calculate stats
   - `nIteration` - prefix `n` to indicate an integer variable
   - `fPatientAge` - `f` to indicate a float variable
   - `sPatientName` - `s` to indicate a string variable
   - `vFileNames` - `v` for vector
   - `lColumnNames` - `l` for a list


R notebooks
===========
[R Notebooks](https://bookdown.org/yihui/rmarkdown/notebook.html) allows to create publish-ready documents with text, graphics, and interactive plots. Can be saved as an html, pdf, or a Word document. 

An R Notebook is a document with chunks that can be executed independently and interactively, with output visible immediately beneath the input. The text is formatted using [R Markdown](https://rmarkdown.rstudio.com/authoring_basics.html).


Important concept 1: data.table
========================================================

`Data.table` package is a faster, more efficient [framework](https://cran.r-project.org/web/packages/data.table/vignettes/datatable-intro.html) for data manipulation compared to R's default `data.frame`. It provides a consistent syntax for subsetting, grouping, updating, merging, etc. 


Important concept 2: writing robust code
========================================

Access columns by reference, never by numbers! Avoid hard-coding column names in your code. Column order may change, column names may change.


Importnat concept 3: avoid for loops
====================================

From [R-bloggers](https://www.r-bloggers.com/how-to-avoid-for-loop-in-r/):

> A FOR loop is the most intuitive way to apply an operation to a series by looping through each item one by one, which makes perfect sense logically but should be avoided by useRs given the low efficiency.

Some context about data from our lab
====================================

- Lot's of time-lapse microscopy experiments: taking movies of many cells
- Cells have fluorescent biosensors that measure activities of proteins
- We look at the dynamics of protein activity
- Movies are processed to identify cells, measure the fluorescent signal, track cells over time
- The reulting data: thousands of time series
- Batch image analysis on a computing cluster generates lot's of CSV files
- Postprocessing: merging files from different experimental conditions, cleaning data from outliers, pulling experimental description from other files

Let's go for a **R**ide
=======================


