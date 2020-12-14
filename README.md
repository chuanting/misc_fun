# Some useful commands

- Generate date range using Pandas
```
idx = pd.date_range(start='02/10/2015', end='03/02/2015',freq='30T', closed='left')
```
- Update conda env on Ibex
```
conda env update --prefix ./env --file environment.yml  --prune
```
- Delete some row that contain specific string
```
sed '/abc/d;/efg/d' a.txt > a.log    // 删除含字符串"abc"或“efg"的行，将结果保存到a.log
```
- Give your ML model an interface
```
import gradio as gr

def greet(name):
  return "Hello " + name + "!"

gr.Interface(fn=greet, inputs="text", outputs="text").launch()
```
-Install PyFlux
```
pip install git+https://github.com/RJT1990/pyflux
```

- scripts to combine ARIMA results

```
sed '' *.txt >> 123.csv
```

- Latex commands to make subfigures

```
\begin{figure*}
\centering

\tabskip=0pt
\valign{#\cr
  \hbox{%
    \begin{subfigure}[b]{.65\textwidth}
    \centering
    \includegraphics[width=\textwidth]{world_v7_cut}
    \caption{BSs distribution over the world.}
    \end{subfigure}%
  }\cr
  \noalign{\hfill}
  \hbox{%
    \begin{subfigure}{.35\textwidth}
    \centering
    \raisebox{.2\textwidth}{
    \includegraphics[width=0.95\textwidth]{fig_2_all}
    }
    \caption{Left: CDF. Right: PDF}
    \end{subfigure}%
  }\cr
}
\caption{Full caption}

\end{figure*}

```