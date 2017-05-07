# paperwriting

# latex

### adjust equation font
change to small, then switch back to normal
```math
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
```latex
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

### table resize
```latex
\begin{table}[h]
\centering
\caption{Compute-intensive Kernels}
\label{tab_compute}
\resizebox{0.95\columnwidth}{!}{%
\begin{tabular}{|l|l|l|}
\hline
\multicolumn{1}{|l|}{\textbf{Kernel Name}} & 
\multicolumn{1}{l|}{\textbf{Application}} & 
\multicolumn{1}{l|}{\textbf{Domain}} \\ \hline
fwtbatch2kernel & fastWalshTransform & computational mathematics \\ \hline
mergeranksandindiceskernel & mergeSort & sorting \\ \hline
mergesortsharedkernel & mergeSort & sorting \\ \hline
\end{tabular}%
}
\end{table}
```
