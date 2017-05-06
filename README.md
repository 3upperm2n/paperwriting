# paperwriting

# latex

### adjust equation font
change to small, then switch back to normal
```
\small
\begin{equation}
warp\_fp32 = inst\_fp\_32 / total\_threads
\end{equation}
\begin{equation}
warp\_fp64 = inst\_fp\_64 / total\_threads
\end{equation}
\begin{equation}
warp\_int = inst\_integer / total\_threads
\end{equation}
\normalsize
```

### align equation and label them
```
\small
\begin{align}
warp\_fp32 &= inst\_fp\_32 / total\_threads \label{eq1} \\
warp\_fp64 &= inst\_fp\_64 / total\_threads \\
warp\_int &= inst\_integer / total\_threads \\
warp\_ldst &= inst\_compute\_ld\_st/ total\_threads \\
warp\_gld &= gld\_transactions/ total\_threads \\
warp\_gst &= gst\_transactions/ total\_threads \\
warp\_smld &= smld\_transactions/ total\_threads \\
warp\_smst &= smst\_transactions/ total\_threads \label{eq8}
\end{align}
\normalsize
```
