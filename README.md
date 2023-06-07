# Using TikZ and PGF to Plot in LaTeX
This repository shares TikZ coding (written by Ian He and JaeSeok Oh) to create plots in LaTeX. To see the coding for each plot in the following section, please click the figure and the hyperlink will lead you to our corresponding tex file. Comments are always welcomed.

**Contact:**

:disguised_face: Ian: ianho0815@outlook.com.
  
:sunglasses: JaeSeok: jaeseok@ou.edu.

## Introduction
TikZ and PGF are languages commonly used in [LaTeX](https://www.latex-project.org/) for producing vector graphics, with lots of wonderful features including the drawing of points, lines, arrows, and shapes. More precisely, PGF is a lower-level language, while TikZ is a set of higher-level macros that use PGF.

To replicate the plots we create in the following sections, you must type the codes below in your LaTeX preamble.
```latex
\usepackage{graphicx, float, asymptote, pgfplots}
\pgfplotsset{compat=1.18}
\usetikzlibrary{calc, calligraphy, decorations.pathreplacing, patterns, shapes.misc}
```
**Note:**
 * The `graphicx` package ([documentation](https://ctan.org/pkg/graphicx)) provides some useful optional arguments to the `\includegraphics` command.
 * The `float` package ([documentation](https://ctan.org/pkg/float)) improves the interface for defining floating objects, such as figures and tables. By default, we can use something `[h]` (here), `t` (top), and `b` (bottom) to determine the figure positioning; however, these positioning options are not strong --- LaTeX still has some flexibility to select the best position in its mind. To precisely fix the position of a floating objects, we have to use the parameter `[H]` from `float`.
 * The `asymptote` package ([documentation](https://ctan.org/pkg/asymptote)) provides a lot of commands for 2D and 3D high-quality level technical drawing.
 * The `pgfplots` package ([documentation](https://ctan.org/pkg/pgfplots)) allows us to draw high-quality function plots. In particular, it supports axis scaling, axis ticks custimization, axis labels custimization, legend entries, etc. Note that `pgfplots` has been written with backwards compatibility; thus, new features occasionally lead to a different behavior. Therefore, we suggest to activate explicitly new features or bugfixes by writing `\pgfplotsset{compat=1.18}` in your preamble, where `compat=1.18` is the highest compatibility level nowadays. The lowest level is `compat=1.3`.
 * `asymptote` and `pgfplots` provide basic functionalities and load the `tikz` and `pgf` packages ([documentation](https://www.ctan.org/pkg/pgf)) automatically. For special features, special libraries must be included. The libraries we use include
   * `calc` (making complex coordinate calculations);
   * `calligraphy` (enabling calligraphic style drawings);
   * `decorations.pathreplacing` (defining decorations that replace the to-be-decorated path by another path);
   * `patterns` (providing different patterns for filling in area);
   * `shapes.misc` (defining additional shapes).


## Functions

### Leontief Production Function
[<img src="https://github.com/IanHo2019/TikZ_Plotting/blob/main/Figures_(Functions)/Leontief_Production_Function.png" title="Leontief Production Function" alt="Leontief Production Function" width="435.9" height="349.2"/>](./Coding/Leontief_Production_Function.tex)
