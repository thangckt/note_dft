This book serves two purposes:

1) to provide worked examples of using DFT to model materials' properties, and
2) to provide references to more advanced treatments of these topics in the literature.

It is not a definitive reference to density functional theory. Along the way to learning how to perform the calculations, you will learn how to analyze the data, make plots, and how to interpret the results. This book is very much "recipe" oriented, with the intention of giving you enough information and knowledge to start your research. In that sense, many of the computations are not publication quality with respect to convergence of calculation parameters.

You will read a lot of python code in this book. I believe that computational work should always be scripted. Scripting provides a written record of everything you have done, making it more probable you (or others) could reproduce your results or report the method of its execution exactly at a later time.

This book makes heavy use of many computational tools including:

Python
Module index
Atomic Simulation Environment (ase)
numpy
scipy
matplotlib
emacs
org-mode This book is written in org-mode, and is best read in emacs in org-mode. This format provides clickable links, easy navigation, syntax highlighting, as well as the ability to interact with the tables and code. The book is also available in PDF.
git This book is available at <https://github.com/jkitchin/dft-book>
vasp This is the Python module used extensively here. It is available at <https://github.com/jkitchin/vasp>
The DFT code used primarily in this book is VASP.

VASP wiki
VASP Manual
Similar code would be used for other calculators, e.g. GPAW, Jacapo, etc… you would just have to import the python modules for those codes, and replace the code that defines the calculator.
