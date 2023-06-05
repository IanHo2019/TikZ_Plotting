# Using TikZ and PGF to Plot in LaTeX
This repository shares TikZ coding (written by Ian He and JaeSeok Oh) to create plots in LaTeX. Comments on better coding or error correction are welcomed.

**Contact:**
  * Ian: ianho0815@outlook.com.
  * JaeSeok: jaeseok@ou.edu.

## Introduction
TikZ and PGF are languages commonly used in [LaTeX](https://www.latex-project.org/) for producing vector graphics, with lots of wonderful features including the drawing of points, lines, arrows, and shapes. More precisely, PGF is a lower-level language, while TikZ is a set of higher-level macros that use PGF.

To replicate the plots we create in the following sections, you must type the codes below in your LaTeX preamble.
```latex
\usepackage{float, asymptote, pgfplots}
\pgfplotsset{compat=1.18}
\usetikzlibrary{calc, calligraphy, decorations.pathreplacing, patterns, shapes.misc}
```

## Functions

### Leontief Production Function
[<img src="https://github.com/IanHo2019/TikZ_Plotting/blob/main/Figures_(Functions)/Leontief_Production_Function.png" title="Leontief Production Function" alt="Leontief Production Function" width="435.9" height="349.2"/>](./Coding/Leontief_Production_Function.txt)
