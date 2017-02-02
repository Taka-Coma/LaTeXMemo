# LaTeXMemo

* Copyright (c) 2016 Takahiro Komamizu
* License: MIT
* Author homepage: https://takacomaprofile.wordpress.com/

# Memos

## Shorten spaces b/w lines of references
```
\usepackage{setspace}
...
\begin{spacing}{0.9}
\bibliography{bibfile}
\end{spacing}
```

## Change title of reference in LaTeX
- ref. http://www.lightstone.co.jp/latex/kb0059.htm
```
\renewcommand{\refname}{XXXXXXXX}
or
\renewcommand{\bibname}{XXXXXXXX}
```

## US letter size setting in ACM format.
```
\setlength{\paperheight}{11in}
\setlength{\paperwidth}{8.5in}
\usepackage[pass, ]{geometry}
```

## ~~Include DOI to ACM format~~ 
- ~~ref. http://www.sheridanprinting.com/typedept/cikm.htm~~
- New ACM format makes it easy > http://www.acm.org/publications/proceedings-template

## Reset the numbering of subfigure in LaTeX
```
\setcounter{subfigure}{0}
```

## Underline with automatic change line
```
\usepackage{soul} 
....
\ul{text}
```

## Arrow with text in Latex
```
\xrightarrow{text}
```
* Dashes
  * `-` for short
  * `--` for middle
* Circle symbol
```
\circ
```

## Add parentheses around subfig references
- ref. http://tex.stackexchange.com/questions/16291/adding-parentheses-around-subfig-references
```
\usepackage[subrefformat=parens,labelformat=parens]{subfig}
...
\subref*{ref}
```

## Use `\url{...}` in `\caption` of table
```
\caption{...\protect\url{...}...}
```

## Shorten left margin of `itemize/enumerate/description`
```
\usepackage{enumitem}
...
\begin{itemize}[leftmargin=*]
...
\end{...}
```

## LaTeX: nice arranging package of PDF pages
```
\usepackage{geometry}
\geometry{
    a4paper,
    total={170mm,257mm},
    left=20mm,
    top=20mm,
}
```

## Footnote in the table and tabular env. 
```
\usepackage{footnote}
\makesavenoteenv{table}
\makesavenoteenv{tabular}
```

## Norm in math mode
```
\lVert ... \rVert
```

## Any font size
```
\usepackage{anyfontsize}
...
{\fontsize{6.5}{6.5}\selectfont
...
}
```
